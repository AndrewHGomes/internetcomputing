<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Polilinhas na Computação Gráfica</h2>

<Audios modulo="M7" aulas={["09", "10", "11", "12"]} />

<p>
  A construção de imagens tridimensionais utiliza descritores vetoriais e
  transformações geométricas para representar objetos do mundo real. Enquanto
  formas regulares como círculos e retas dependem de poucos parâmetros,
  estruturas complexas exigem uma abordagem baseada em pontos relacionados para
  lidar com a complexidade das formas.
</p>

<p>
  Uma <strong>polilinha</strong> é definida como um conjunto de vértices conectados
  por segmentos de reta. Ela funciona como uma técnica de aproximação para representar
  linhas curvas e formas irregulares. Na prática, uma curva contínua é decomposta
  em várias pequenas retas que, juntas, delineiam a forma desejada.
</p>

<h3>Fidelidade vs. Desempenho</h3>

<p>
  A qualidade da representação de uma polilinha depende diretamente da
  quantidade de segmentos utilizados. Existe um equilíbrio necessário entre a
  precisão visual e o custo computacional:
</p>

<ul>
  <li>
    <strong>Baixo número de segmentos:</strong> Consome menos memória e processamento,
    mas resulta em uma representação serrilhada ou grosseira da forma original.
  </li>
  <li>
    <strong>Alto número de segmentos:</strong> Proporciona maior fidelidade e suavidade
    à curva, porém exige mais recursos do hardware para armazenamento e renderização.
  </li>
</ul>

<p>
  Em termos de implementação, as polilinhas são tratadas em linguagens de
  programação como sequências de vértices, onde cada ponto é definido por suas
  coordenadas espaciais. Essa estrutura permite a criação de polígonos e a base
  para modelos geométricos mais avançados.
</p>

<h3>Splines</h3>

<p>
  Enquanto as polilinhas utilizam segmentos de reta, as <strong>splines</strong>
  são curvas compostas por seções polinomiais que mantêm continuidade em suas junções.
  Elas permitem representar formas curvas de maneira suave e matematicamente precisa.
</p>

<p>
  Um polinômio é uma soma de parcelas que, graficamente, resulta em curvas
  suaves. Um polinômio de ordem 3, por exemplo, pode ser descrito por apenas
  quatro parâmetros. Sua representação matemática segue o formato:
</p>

<ul>
  <li>f(x) = ax<sup>3</sup> + bx<sup>2</sup> + cx + d</li>
</ul>

<p>
  Essa mesma função pode ser expressa em forma matricial para facilitar o
  processamento computacional:
</p>

<ul>
  <li>f(x) = [x<sup>3</sup> x<sup>2</sup> x 1] * [a b c d]<sup>T</sup></li>
</ul>

<h4>Curvas de Bézier</h4>

<p>
  As curvas de Bézier utilizam <strong>pontos de controle</strong> para definir a
  trajetória da curva. Elas são amplamente aplicadas em design e modelagem industrial.
  A definição matemática da curva é dada por:
</p>

<ul>
  <li>C(t) = Σ<sub>i=0</sub><sup>n</sup> P<sub>i</sub> B<sub>i,n</sub>(t)</li>
</ul>

<p>
  Nesta fórmula, P<sub>i</sub> representa os pontos de controle e B<sub>i,n</sub
  >(t) são os polinômios de Bernstein. Na prática, o computador interpreta esses
  pontos de controle para gerar a curvatura suave entre eles.
</p>

<h4>B-Splines e Superfícies</h4>

<p>
  As <strong>B-Splines</strong> são variações mais complexas que oferecem uma vantagem
  técnica: o grau do polinômio pode ser definido independentemente do número de pontos
  de controle. Isso garante maior flexibilidade na modelagem de objetos detalhados.
</p>

<ul>
  <li>
    <strong>Representação:</strong> Assim como as polilinhas, as splines são armazenadas
    na memória como sequências de vértices (pontos de controle), mas o resultado
    visual é uma curva real e contínua.
  </li>
  <li>
    <strong>Superfícies:</strong> O conceito pode ser expandido do plano 2D para
    o espaço 3D, criando superfícies de Bézier ou superfícies B-Spline. Nesses casos,
    os pontos de controle definem "malhas" que moldam superfícies tridimensionais
    complexas.
  </li>
</ul>

<h3>Poliedros e Malhas</h3>

<p>
  Na computação gráfica 3D, sólidos contínuos são aproximados por estruturas
  simplificadas chamadas <strong>poliedros</strong>. Um poliedro é um sólido
  constituído por um arranjo de pequenas faces formadas por polígonos planares.
  O conjunto dessas faces é denominado <strong>malha poligonal</strong>, podendo
  representar superfícies abertas ou fechadas.
</p>

<h4>Classificação de Polígonos</h4>

<p>
  Para entender a construção das malhas, é necessário classificar os polígonos
  que as compõem:
</p>

<ul>
  <li>
    <strong>Simples:</strong> Polígonos onde não há interseção entre os segmentos
    de reta que formam suas arestas.
  </li>
  <li>
    <strong>Não-simples:</strong> Polígonos que possuem interseção entre seus segmentos.
  </li>
  <li>
    <strong>Convexos:</strong> Polígonos onde qualquer segmento de reta ligando dois
    pontos internos permanece totalmente dentro da figura. São os preferidos na computação
    gráfica por facilitarem cálculos de exibição.
  </li>
</ul>

<h4>Malhas Poligonais e Representação</h4>

<p>
  As malhas poligonais (como a representação de uma esfera ou de objetos
  complexos) são compostas por triângulos ou quadriláteros. Embora modelos
  possam conter diversos tipos de polígonos, é comum converter toda a malha em
  <strong>triângulos</strong> por dois motivos principais:
</p>

<ol>
  <li>
    <strong>Garantia de Convexidade:</strong> Triângulos são, por definição, convexos
    e planares, eliminando problemas com concavidades.
  </li>
  <li>
    <strong>Eficiência de Memória:</strong> Malhas triangulares possuem estruturas
    de dados mais simples, otimizando o desempenho dos algoritmos de manipulação
    e renderização em telas 2D.
  </li>
</ol>

<h4>Armazenamento</h4>

<p>
  A escolha da estrutura de dados para armazenar essas malhas na memória do
  computador é crucial, pois define a velocidade com que o sistema consegue
  processar transformações geométricas e a visualização final do objeto.
</p>

<h3>Visão e Cores</h3>

<p>
  O sistema visual humano é a base para a computação gráfica. A retina possui
  duas células principais: os <strong>bastonetes</strong> (visão em baixa luz e
  preto-e-branco) e os <strong>cones</strong> (visão de cores). Os três tipos de
  cones humanos são sensíveis ao vermelho, verde e azul, o que fundamenta a criação
  de modelos digitais.
</p>

<h4>Modelo RGB (Aditivo)</h4>

<p>
  Utilizado em telas e dispositivos que emitem luz, o modelo RGB baseia-se na
  adição de cores primárias: <strong
    >Vermelho (Red), Verde (Green) e Azul (Blue)</strong
  >. A mistura dessas luzes resulta em:
</p>

<ul>
  <li>
    <strong>Secundárias:</strong> Verde + Vermelho = Amarelo; Vermelho + Azul = Magenta;
    Verde + Azul = Ciano.
  </li>
  <li><strong>Branco (W):</strong> Soma de Verde + Vermelho + Azul.</li>
  <li>
    <strong>Representação:</strong> Cada cor é um vetor (r, g, b) com valores de
    0 a 255.
  </li>
</ul>

<p>
  O <strong>Cubo RGB</strong> ilustra esse sistema espacialmente. A origem do
  cubo representa o preto (K), enquanto o vértice oposto é o branco (W). A
  diagonal entre eles representa a escala de cinza. Adicionalmente, imagens
  digitais podem incluir um canal de <strong>transparência</strong> (canal Alpha),
  que controla a opacidade na sobreposição de imagens.
</p>

<h4>Modelo CMYK (Subtrativo)</h4>

<p>
  Empregado na impressão física, o modelo CMYK funciona pela subtração de luz
  refletida em pigmentos. Suas cores básicas são as secundárias do RGB: <strong>
    Ciano (C), Magenta (M) e Amarelo (Y)
  </strong>.
</p>

<ul>
  <li>A mistura de C, M e Y resulta na ausência de luz refletida (Preto).</li>
  <li>
    O <strong>Preto (K)</strong> é adicionado como um pigmento separado por economia
    e precisão técnica, evitando o uso excessivo das outras tintas para formar tons
    escuros.
  </li>
</ul>

<h4>Outros Modelos de Cor</h4>

<p>
  Além dos modelos baseados em hardware (telas/impressoras), existem modelos
  baseados na percepção humana:
</p>

<ul>
  <li>
    <strong>HSL:</strong> Define a cor por Matiz (H - cor pura), Saturação (S - intensidade)
    e Luminância (L - brilho). É ideal para algoritmos de processamento de imagem
    que precisam ordenar cores.
  </li>
  <li>
    <strong>Variantes:</strong> HSI, HSV, Lab e YCbCr são utilizados em contextos
    específicos de compressão e tratamento de imagem.
  </li>
</ul>

<h3>Visão Estéreo</h3>

<p>
  A <strong>visão estéreo</strong> é a técnica que permite a percepção de profundidade
  a partir de imagens bidimensionais. O cérebro humano processa as informações capturadas
  pelos dois olhos (visão binocular) e as funde em uma única percepção tridimensional.
  No entretenimento, o termo "3D" geralmente refere-se à projeção simultânea de duas
  imagens 2D capturadas por câmeras de lentes duplas.
</p>

<h4>Técnicas de Visualização</h4>

<p>
  A evolução da visão estéreo no cinema e em telas seguiu diferentes métodos
  para garantir que cada olho receba apenas a imagem que lhe é destinada:
</p>

<ul>
  <li>
    <strong>Anáglifo:</strong> Técnica clássica que utiliza filtros de cores (geralmente
    vermelho e ciano). As imagens são sobrepostas com cores complementares, e os
    óculos coloridos filtram a luz para que cada olho veja uma perspectiva diferente.
    A desvantagem principal é a alteração nas cores originais da cena (aberração
    cromática).
  </li>
  <li>
    <strong>Polarização da Luz:</strong> Método moderno que substitui as cores por
    diferentes ângulos de vibração da luz. As imagens são projetadas com polarizações
    distintas (ex: horizontal e vertical), e os óculos polarizadores garantem a separação
    sem distorcer as cores.
  </li>
  <li>
    <strong>Barreira de Paralaxe:</strong> Tecnologia promissora que dispensa o uso
    de óculos. Utiliza um anteparo físico sobre a tela com ranhuras finas que direcionam
    partes específicas da imagem (entrelaçadas) para cada olho, baseando-se na distância
    entre eles.
  </li>
</ul>

<h4>Conceito de Profundidade</h4>

<p>
  É importante destacar que o cinema 3D não projeta objetos volumétricos reais,
  mas sim engana o sistema visual ao fornecer o <strong>paralaxe</strong> necessário
  para que o cérebro reconstrua a profundidade. Se a captura ou a projeção falharem
  em alinhar essas duas perspectivas, o efeito tridimensional é perdido.
</p>

<h3>Conclusão</h3>

<p>
  Esta etapa consolidou os fundamentos da computação gráfica, desde a modelagem
  de formas geométricas até as tecnologias de exibição e percepção visual.
</p>

<h4>Modelagem de Formas e Estruturas</h4>

<p>
  A representação de objetos no espaço digital evolui de segmentos simples para
  malhas complexas:
</p>

<ul>
  <li>
    <strong>Polilinhas:</strong> Fundamentais para descrever formas não regulares.
    O nível de fidelidade ao modelo original é ditado pelo número de vértices; quanto
    mais pontos, maior a precisão da curva, porém maior é o custo de processamento
    e memória.
  </li>
  <li>
    <strong>Splines:</strong> Modelagens baseadas em funções polinomiais para
    criar curvas suaves. Destacam-se as <strong>Curvas de Bézier</strong> e as
    <strong>B-Splines</strong>, que permitem construir trajetórias curvas de
    forma simples, apesar da complexidade matemática subjacente.
  </li>
  <li>
    <strong>Poliedros e Malhas:</strong> Estruturas complexas formadas pela
    agregação de polígonos planares. Na computação gráfica, dá-se preferência ao
    uso de <strong>triângulos</strong>
    para compor essas malhas, devido à sua eficiência computacional.
  </li>
</ul>

<h4>Visão, Cores e Profundidade</h4>

<p>
  O processo final envolve como a imagem é entregue ao sistema visual humano:
</p>

<ul>
  <li>
    <strong>Sistemas de Cores:</strong> A aula focou nos dois modelos
    principais: o <strong>RGB</strong> (aditivo), baseado na emissão de luz para
    telas, e o <strong>CMYK</strong> (subtrativo), baseado na absorção de pigmentos
    para impressões.
  </li>
  <li>
    <strong>Visão Estéreo:</strong> Técnica que simula a tridimensionalidade utilizando
    duas imagens simultâneas para enganar o cérebro. Os métodos atuais incluem o
    uso de filtros de cor (óculos coloridos) e sistemas de luz polarizada (óculos
    polarizadores).
  </li>
</ul>
