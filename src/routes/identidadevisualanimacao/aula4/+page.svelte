<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Câmera Virtual</h2>

<Audios modulo="M7" aulas={["13", "14", "15", "16"]} />

<p>
  A câmera virtual é o conceito que permite projetar modelos 3D armazenados na
  memória do computador em uma tela bidimensional, simulando o funcionamento de
  uma câmera fotográfica real. Para que essa projeção ocorra, é necessário
  definir o posicionamento do observador e aplicar transformações geométricas
  nos polígonos da cena.
</p>

<h3>Parâmetros e Graus de Liberdade</h3>

<p>
  O posicionamento e a movimentação da câmera virtual são definidos por <strong>
    sete graus de liberdade
  </strong>, que determinam como ela interage com o ambiente:
</p>

<ul>
  <li>
    <strong>Translação:</strong> Movimentação ao longo dos eixos x, y e z.
  </li>
  <li><strong>Rotação:</strong> Giro em torno dos eixos x, y e z.</li>
  <li><strong>Foco:</strong> Ajuste da distância focal (f).</li>
</ul>

<h4>Sistemas de Coordenadas e Projeção</h4>

<p>
  O processo de visualização exige a transição entre diferentes sistemas de
  referência:
</p>

<ol>
  <li>
    <strong>Mundo Real (3D):</strong> Os objetos estão posicionados e orientados
    em um espaço x, y, z.
  </li>
  <li>
    <strong>Sistema da Câmera:</strong> Os objetos são transformados (transladados
    e rotacionados) para a perspectiva específica da câmera escolhida.
  </li>
  <li>
    <strong>Tela de Projeção (2D):</strong> Através de transformações geométricas,
    os pontos do espaço 3D são projetados em um plano 2D (x, y).
  </li>
</ol>

<p>
  Diferente de uma captura simples de pontos, a síntese final da imagem deve
  considerar elementos adicionais que dão realismo à cena, como a textura dos
  objetos e a iluminação do ambiente.
</p>

<h3>Síntese de Imagens</h3>

<p>
  A síntese de imagens foca na criação de imagens artificiais — isoladas ou
  integradas a vídeos reais — unindo conceitos de geometria, iluminação e
  texturização. O processo transforma modelos matemáticos em representações
  visuais.
</p>

<h4>Modelo de Câmera e Matriz de Projeção</h4>

<p>
  Para projetar um modelo 3D em um plano 2D, utiliza-se o sistema de coordenadas
  do mundo real como referência. A posição e orientação da câmera são
  controladas por uma matriz de transformação M, que atua como o "comando" da
  câmera virtual:
</p>

<ul>
  <li>M = P * T<sub>2</sub> * R<sub>y</sub> * R<sub>x</sub> * T<sub>1</sub></li>
</ul>

<p>Nesta composição:</p>

<ul>
  <li>
    <strong><b>T<sub>1</sub>:</b></strong> Translação do sistema de coordenadas do
    mundo para o da câmera.
  </li>
  <li>
    <strong><b>R<sub>x</sub></b> e R<sub>y</sub>:</strong> Rotações em torno dos
    eixos para definir o direcionamento.
  </li>
  <li>
    <strong><b>T<sub>2</sub>:</b></strong> Translação secundária para ajuste do sistema.
  </li>
  <li>
    <strong><b>P:</b></strong> Transformação de perspectiva, responsável pelo efeito
    de aproximação ou afastamento.
  </li>
</ul>

<h4>Pipeline de Visualização (Renderização)</h4>

<p>
  O pipeline de renderização é um processo sequencial onde a saída de uma etapa
  serve de entrada para a próxima. Seus componentes fundamentais são: vértices,
  malhas poligonais, texturas, câmera virtual e iluminação. Os estágios
  principais incluem:
</p>

<ol>
  <li>
    <strong>Transformações Geométricas:</strong> Aplicadas aos vértices das malhas
    para posicionar e rotacionar os objetos na cena.
  </li>
  <li>
    <strong>Câmera Virtual:</strong> Aplicação de transformações em todos os vértices
    (exceto a perspectiva final) para alinhar a cena ao ponto de vista do observador.
  </li>
  <li>
    <strong>Adição de Atributos:</strong> Inclusão de informações de textura e iluminação
    em cada face das malhas.
  </li>
  <li>
    <strong>Rasterização:</strong> Processo que projeta os pontos em perspectiva
    e gerencia oclusões (quando um objeto esconde outro), gerando fragmentos da imagem.
  </li>
  <li>
    <strong>Montagem da Imagem:</strong> Estágio final que compõe os fragmentos na
    imagem digital definitiva.
  </li>
</ol>

<p>
  O sistema permite <strong>interação do usuário</strong>, possibilitando o
  ajuste de objetos, troca de pontos de vista e criação de animações em tempo
  real através de realimentações no pipeline.
</p>

<h3>Rasterização</h3>

<p>
  A rasterização é o processo de converter a geometria contínua de um objeto 3D
  em uma grade finita de pixels para exibição em tela. Como é impossível
  calcular infinitos pontos de luz em uma cena, a computação utiliza estratégias
  para processar apenas o que é visível e necessário.
</p>

<h4>O Algoritmo Ray Casting</h4>

<p>
  Para resolver o problema da visibilidade e projeção, utiliza-se o <strong
    >ray casting</strong
  >. Diferente da física real, onde a luz viaja da fonte para o olho, este
  algoritmo inverte o sentido para economizar processamento:
</p>

<ol>
  <li>
    <strong>Grade de Projeção:</strong> Define-se uma tela virtual (malha) entre
    o observador e a cena.
  </li>
  <li>
    <strong>Lançamento de Raios:</strong> Dispara-se um raio imaginário partindo
    do olho do observador, passando por cada ponto (pixel) da malha em direção aos
    objetos.
  </li>
  <li>
    <strong>Interseção e Oclusão:</strong> O algoritmo identifica quais polígonos
    o raio atinge. Se um raio intercepta múltiplos objetos, apenas o ponto mais próximo
    do observador define a cor do pixel, tratando automaticamente as oclusões (objetos
    escondidos atrás de outros).
  </li>
  <li>
    <strong>Mapeamento:</strong> A cor calculada na tela virtual é transferida para
    as coordenadas da tela física.
  </li>
</ol>

<h4>Ray Casting vs. Ray Tracing</h4>

<p>
  Embora os nomes sejam parecidos, a diferença reside na eficiência e no nível
  de detalhamento:
</p>

<ul>
  <li>
    <strong>Ray Casting:</strong> É mais econômico. Ele lança raios e pode agrupar
    cálculos com base em restrições geométricas (como superfícies uniformes), não
    rastreando necessariamente cada raio de forma independente após o primeiro impacto.
  </li>
  <li>
    <strong>Ray Tracing:</strong> Cada raio é rastreado individualmente e pode gerar
    novos raios (reflexões, refrações) ao atingir superfícies. Cada pixel é o resultado
    de um rastreamento detalhado, oferecendo maior realismo ao custo de maior poder
    computacional.
  </li>
</ul>

<h4>Determinação da Cor</h4>

<p>
  A cor final de um ponto P<sub>T</sub> na tela é influenciada por uma combinação
  de fatores:
</p>

<ul>
  <li>Posição do observador (V).</li>
  <li>Posição e intensidade da fonte de luz.</li>
  <li>Inclinação (normal) e propriedades do material do polígono atingido.</li>
</ul>

<h3>Visualização: Modelo de Phong</h3>

<p>
  O <strong>Modelo de Phong</strong> é um dos algoritmos mais utilizados para simular
  a interação da luz com superfícies em computação gráfica. Ele decompõe a luminosidade
  de um ponto em três componentes principais, permitindo imitar materiais que variam
  de foscos a metálicos.
</p>

<h4>Os Três Componentes de Iluminação</h4>

<ol>
  <li>
    <strong>Reflexão Ambiente (I<sub>a</sub>):</strong> Representa a luz que já
    foi refletida tantas vezes pelo ambiente que atinge o objeto de todas as
    direções. É uma aproximação simplificada da iluminação global.
    <ul>
      <li>Fórmula: I<sub>a</sub> = K<sub>a</sub> * I<sub>amb</sub></li>
    </ul>
  </li>
  <li>
    <strong>Reflexão Difusa (I<sub>d</sub>):</strong> Ocorre em superfícies
    foscas ou rugosas. A luz incide e se espalha uniformemente em todas as
    direções. Sua intensidade depende do ângulo entre a fonte de luz e a normal
    da superfície.
    <ul>
      <li>
        Fórmula: I<sub>d</sub> = K<sub>d</sub> * I<sub>in</sub> * cos(θ)
      </li>
    </ul>
  </li>
  <li>
    <strong>Reflexão Especular (I<sub>s</sub>):</strong> Cria o "ponto de
    brilho" (highlight) em objetos polidos. A luz reflete em uma direção
    preferencial, agindo como um espelho.
    <ul>
      <li>
        Fórmula: I<sub>s</sub> = K<sub>s</sub> * I<sub>in</sub> * cos<sup>n</sup
        >(φ)
      </li>
    </ul>
  </li>
</ol>

<h4>Parâmetros do Material</h4>

<p>
  O realismo do objeto depende de coeficientes intrínsecos definidos no modelo
  3D:
</p>

<ul>
  <li>
    <strong>K<sub>a</sub>, K<sub>d</sub>, K<sub>s</sub>:</strong> Coeficientes de
    reflexão (ambiente, difusa e especular). Definem a proporção de luz que o objeto
    reflete ou absorve.
  </li>
  <li>
    <strong>Expoente de Brilho (n):</strong> Define a "polidez". Um <b>n</b>
    alto (esfera de aço) gera um brilho pequeno e intenso; um <b>n</b> baixo (bola
    de tênis) gera um brilho espalhado e suave.
  </li>
  <li>
    <strong>Atenuação:</strong> A intensidade da luz direta (<b
      >I<sub>in</sub></b
    >) diminui conforme a distância entre a fonte e o objeto aumenta.
  </li>
</ul>

<h4>O Modelo Completo</h4>

<p>
  Para uma cena com N fontes de luz, a intensidade total de cor (para cada canal
  R, G e B) é a soma das componentes:
</p>

<ul>
  <li>
    I<sub>total</sub> = I<sub>a</sub> + Σ<sub>i=1</sub><sup>N</sup> (I<sub
      >d,i</sub
    >
    + I<sub>s,i</sub>)
  </li>
</ul>

<p>
  Essa soma garante que o objeto tenha uma cor base (ambiente), volume e
  sombreamento (difusa) e pontos de brilho (especular), resultando em uma
  percepção tridimensional convincente.
</p>

<h3>Visualização: Tonalização e Textura</h3>

<p>
  Os modelos de <strong>tonalização</strong> (shading) definem como a luz e as cores
  são distribuídas pelas faces dos polígonos. Enquanto o modelo de Phong calcula
  a cor de um ponto, a tonalização determina como esses cálculos são aplicados em
  toda a superfície do objeto para aumentar o realismo sem necessariamente exigir
  um número excessivo de polígonos.
</p>

<h4>Tonalização Constante vs. Interpolada</h4>

<p>
  A forma como os polígonos são sombreados altera drasticamente a percepção de
  suavidade do objeto:
</p>

<ul>
  <li>
    <strong>Tonalização Constante (Flat Shading):</strong> Cada polígono recebe uma
    cor única e uniforme baseada na sua normal. O resultado é um objeto com aparência
    "facetada", onde as bordas entre os polígonos são claramente visíveis.
  </li>
  <li>
    <strong>Tonalização Interpolada (Smooth Shading):</strong> Utiliza o
    conceito de superfícies curvas (baseado em <strong>splines</strong>) para
    calcular a iluminação. Em vez de tratar a face como plana, o algoritmo
    interpola as normais ou as cores dos vértices vizinhos. Isso cria uma
    transição suave de luz e sombra, simulando uma superfície curva mesmo em
    modelos com poucos polígonos.
  </li>
</ul>

<h4>Texturização</h4>

<p>
  A <strong>textura</strong> é uma técnica fundamental para adicionar detalhes complexos
  (como rugosidade, estampas ou porosidade) sem aumentar a contagem de polígonos.
</p>

<ul>
  <li>
    <strong>Definição:</strong> É uma imagem bidimensional (mapa de bits) aplicada
    sobre a face de um polígono, funcionando como um "papel de parede" digital.
  </li>
  <li>
    <strong>Mapeamento:</strong> Para definir a cor de um ponto interno do polígono,
    o computador realiza o mapeamento das coordenadas dos vértices do polígono sobre
    as coordenadas da imagem de textura (coordenadas UV).
  </li>
  <li>
    <strong>Resultado:</strong> Permite que objetos simples apresentem detalhes visuais
    ricos, como a textura de uma rocha, madeira ou a pele de um personagem, extraindo
    as cores diretamente da imagem de referência.
  </li>
</ul>

<h3>Conclusão</h3>

<p>
  Esta etapa focou no processo de transformação de dados matemáticos
  tridimensionais em imagens digitais visíveis, detalhando desde o
  posicionamento do observador até o acabamento visual das superfícies.
</p>

<h4>Câmera Virtual e Síntese</h4>

<p>
  A <strong>câmera virtual</strong> é o ponto de origem para a visualização. Seu
  posicionamento é controlado por <strong>sete graus de liberdade</strong>
  (translação, rotação e foco). Na síntese de imagens, esse processo é consolidado
  no <strong>pipeline de visualização</strong>, que organiza sequencialmente os
  vértices, malhas e transformações geométricas para alinhar a cena ao ponto de
  vista desejado.
</p>

<h4>Rasterização via Ray Casting</h4>

<p>
  Como a tela de exibição é composta por uma grade finita de pixels, utiliza-se
  a <strong>rasterização</strong> para converter o espaço contínuo em pontos
  discretos. O algoritmo de <strong>ray casting</strong> realiza essa tarefa disparando
  raios imaginários do observador para a cena. Ele determina quais polígonos são
  visíveis em cada pixel e resolve automaticamente as oclusões (objetos escondidos).
</p>

<h4>Modelos de Visualização</h4>

<p>
  Para que o objeto pareça real, três componentes de renderização são aplicados:
</p>

<ul>
  <li>
    <strong>Modelo de Phong:</strong> Calcula a iluminação física, dividindo a
    luz em componentes <strong>ambiente</strong> (base), <strong>difusa</strong>
    (volume/fosco) e <strong>especular</strong> (brilho/reflexo).
  </li>
  <li>
    <strong>Tonalização (Shading):</strong> Define se a superfície parecerá facetada
    (tonalização constante) ou suave e curva (tonalização interpolada), aproximando
    polígonos planos de superfícies suaves via splines.
  </li>
  <li>
    <strong>Texturas:</strong> Aplica imagens bidimensionais (mapas de bits) sobre
    os polígonos, permitindo adicionar detalhes visuais complexos (como padrões de
    madeira ou tecidos) sem aumentar a carga de processamento geométrico.
  </li>
</ul>
