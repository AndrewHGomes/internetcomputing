<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Introdução à Computação Gráfica</h2>

<Audios modulo="M7" aulas={["01", "02", "03", "04"]} />

<p>
  A computação gráfica e o processamento digital de imagens abrangem o estudo de
  ferramentas matemáticas e computacionais voltadas para a criação, manipulação
  e análise de elementos visuais. O foco principal é compreender a geometria da
  construção de imagens, as subáreas de especialização e o funcionamento técnico
  das imagens matriciais.
</p>

<h3>Requisitos de Hardware e Software</h3>

<p>
  Para o desenvolvimento em computação gráfica, a infraestrutura necessária
  varia conforme a aplicação, mas baseia-se em componentes fundamentais de
  processamento e captura.
</p>

<h4>Hardware:</h4>

<ul>
  <li>
    <strong>Microprocessadores (CPU):</strong> Unidades de uso geral para o processamento
    lógico do sistema.
  </li>
  <li>
    <strong>Unidades de Processamento Gráfico (GPU):</strong> Processadores dedicados
    especificamente para acelerar a renderização e o cálculo gráfico.
  </li>
  <li>
    <strong>Dispositivos de Captura:</strong> Câmeras digitais e sensores baseados
    em ondas de rádio, laser ou ultrassom para digitalizar elementos do mundo real.
  </li>
  <li>
    <strong>Interfaces de Imersão:</strong> Óculos e máscaras específicos para aplicações
    de Realidade Virtual (VR) e Realidade Aumentada (AR).
  </li>
</ul>

<h4>Software:</h4>

<ul>
  <li>
    <strong>Bibliotecas e APIs:</strong> Interfaces que permitem aos desenvolvedores
    acessar ferramentas de processamento gráfico de forma interativa.
  </li>
  <li>
    <strong>Softwares de Modelagem e Síntese:</strong> Ferramentas focadas em construção
    3D, animação e visualização de cenários.
  </li>
  <li>
    <strong>Editores de Imagem:</strong> Aplicativos voltados para manipulação direta,
    permitindo segmentação, filtragem e compressão de dados visuais.
  </li>
  <li>
    <strong>Aplicações de Uso Específico:</strong> Sistemas dedicados a áreas restritas,
    como medicina diagnóstica (exames) e processamento de dados de satélites.
  </li>
</ul>

<h3>Conceito e Escopo da Computação Gráfica</h3>

<p>
  A computação gráfica dedica-se ao processamento computacional de elementos
  gráficos em diversos formatos e finalidades. Enquanto o designer utiliza
  ferramentas prontas, o desenvolvedor especializado foca na criação e extensão
  de soluções técnicas, construindo aplicativos e algoritmos que vão além do que
  o mercado oferece. O ciclo básico envolve converter objetos ou cenas do mundo
  real em representações digitais na memória do computador, utilizando modelos
  matemáticos e descritores de imagem para processá-los e exibi-los novamente no
  mundo físico.
</p>

<h4>Processos de Entrada: Modelagem e Captura</h4>

<p>
  O ponto de partida é o mundo real, cujas informações são convertidas para o
  meio eletrônico através de dois métodos principais:
</p>

<ul>
  <li>
    <strong>Modelagem:</strong> Processo de representar objetos por meio de equações,
    funções, pontos, retas e superfícies geométricas. O resultado costuma ser um
    modelo tridimensional criado manualmente ou via softwares específicos.
  </li>
  <li>
    <strong>Captura:</strong> Registro de dados do mundo real através de sensores.
    O exemplo mais comum é a câmera fotográfica (sensor CCD), mas também inclui dispositivos
    que não usam luz visível, como máquinas de ressonância magnética que geram imagens
    a partir de medições específicas.
  </li>
</ul>

<h4>Transformações e Saída de Dados</h4>

<p>
  Para que uma imagem seja exibida ou armazenada, ela passa por processamentos
  baseados em parâmetros matemáticos. Esses modelos permitem realizar
  transformações geométricas, como rotação e translação. Além disso, os dados
  podem passar por um processo de serialização, transformando a descrição visual
  em um arquivo descritor de imagem capaz de ser lido por diferentes sistemas.
</p>

<h4>Realidades e Interações</h4>

<p>
  A disciplina define diferentes níveis de interação entre o ambiente físico e o
  sintético:
</p>

<ul>
  <li>
    <strong>Realidade Material:</strong> O mundo físico puro, sem a presença de imagens
    sintéticas.
  </li>
  <li>
    <strong>Realidade Virtual:</strong> Ambiente totalmente digital que isola o usuário
    da realidade material, criando uma sensação de imersão completa em um novo espaço.
  </li>
  <li>
    <strong>Realidade Aumentada:</strong> Integração que sobrepõe elementos gráficos
    virtuais sobre a imagem capturada do mundo real, combinando ambas as realidades
    na mesma visualização.
  </li>
</ul>

<h4>Aplicações Práticas</h4>

<p>
  A computação gráfica está presente em uma vasta gama de tecnologias
  cotidianas:
</p>

<ul>
  <li>
    <strong>Entretenimento:</strong> Jogos digitais, animações e produções para cinema
    e TV.
  </li>
  <li>
    <strong>Segurança e Biometria:</strong> Leitores de impressão digital e reconhecimento
    facial.
  </li>
  <li>
    <strong>Dispositivos:</strong> Câmeras digitais com filtros e interfaces de toque
    (touchscreen).
  </li>
  <li>
    <strong>Indústria e Ciência:</strong> Modelagem 3D, edição de vídeos e sistemas
    de navegação para robótica.
  </li>
</ul>

<h3>Subáreas da Computação Gráfica</h3>

<p>
  A computação gráfica é dividida em quatro áreas principais, diferenciadas por
  seus objetivos e pelo tipo de dado que entra e sai de cada processamento.
</p>

<h4>Modelagem Tridimensional</h4>

<p>
  O foco é a criação de modelos matemáticos em 3D de objetos ou cenas. Embora
  possa ser feita manualmente, é comum o uso de imagens do mundo real para
  aumentar o realismo. Dispositivos como scanners 3D a laser auxiliam nesse
  processo, enquanto a técnica de reconstrução utiliza imagens 2D capturadas de
  diferentes ângulos para gerar o modelo tridimensional, extraindo também
  informações de cor e textura.
</p>

<h4>Síntese de Imagens</h4>

<p>
  Esta subárea produz imagens sintéticas a partir de modelos matemáticos e
  transformações geométricas. É a base para a criação de interfaces gráficas
  (GUI) e animações. Enquanto o descritor de imagem é apenas um conjunto de
  pontos que descrevem superfícies, a síntese de imagens utiliza construções
  geométricas complexas e digitalização para converter esses dados em imagens
  visíveis em telas.
</p>

<h4>Visão Computacional</h4>

<p>
  Diferente das anteriores, esta área busca extrair informações úteis e análises
  de dados a partir de imagens capturadas do mundo real. O objetivo é obter
  nitidez para identificar objetos de interesse. Para facilitar essa extração, a
  imagem passa por pré-processamentos como filtragem (remoção de ruídos) e
  segmentação (separação de partes da imagem).
</p>

<h4>Processamento de Imagens</h4>

<p>
  Dedicada ao tratamento e alteração de imagens digitais, onde tanto a entrada
  quanto a saída são imagens. O objetivo é modificar a imagem original para
  obter uma versão alterada, abrangendo desde a edição e restauração até a
  preparação para impressão e técnicas de compressão/descompressão de arquivos.
</p>

<h4>Resumo de Entradas e Saídas</h4>

<ul>
  <li>Modelagem 3D: Mundo Real/Imagens &Rarr; Modelos Matemáticos.</li>
  <li>Síntese de Imagens: Modelos Matemáticos &Rarr; Imagem Digital.</li>
  <li>Visão Computacional: Imagem Digital &Rarr; Informação/Descrição.</li>
  <li>
    Processamento de Imagens: Imagem Digital &Rarr; Imagem Digital (alterada).
  </li>
</ul>

<h3>Geometria na Construção de Imagens</h3>

<p>
  A computação gráfica moderna utiliza a geometria analítica (plana e espacial)
  para criar representações digitais. Em vez de pinceladas, formas são geradas a
  partir de coordenadas, equações e funções matemáticas.
</p>

<h4>Retas e Cônicas</h4>

<p>
  A construção de formas básicas no plano cartesiano utiliza equações onde as
  constantes definem as propriedades geométricas da figura:
</p>

<ul>
  <li>
    <strong>Retas:</strong> Geralmente descritas pela equação ax + by + c = 0.
  </li>
  <li>
    <strong>Círculos:</strong> Definidos por (x - x<sub>0</sub>)<sup>2</sup> +
    (y - y<sub>0</sub>)<sup>2</sup> = r<sup>2</sup>, onde r é o raio e (x<sub
      >0</sub
    >, y<sub>0</sub>) é o centro.
  </li>
  <li>
    <strong>Cônicas:</strong>
    Curvas formadas pela interseção de um plano com um cone:
    <ul>
      <li>
        <strong>Elipses:</strong> x<sup>2</sup>/a<sup>2</sup> + y<sup>2</sup
        >/b<sup>2</sup> = 1
      </li>
      <li><strong>Parábolas:</strong> y = ax<sup>2</sup></li>
      <li>
        <strong>Hipérboles:</strong> x<sup>2</sup>/a<sup>2</sup> - y<sup>2</sup
        >/b<sup>2</sup> = 1
      </li>
    </ul>
  </li>
</ul>

<h4>Funções Matemáticas</h4>

<p>
  As funções relacionam elementos de um domínio a um contradomínio para
  construir formas complexas:
</p>

<ul>
  <li>
    <strong>Funções Contínuas:</strong> Utilizam números reais (R). Exemplos incluem
    a função f(x) = sen(x) para ondas ou f(x,y) = sen(x) + cos(y) para superfícies
    tridimensionais.
  </li>
  <li>
    <strong>Funções Discretas:</strong> Utilizam números inteiros (Z). Os pontos
    não são contínuos, sendo úteis para representações que se assemelham a grades.
  </li>
</ul>

<h4>Vetores e Imagens Digitais</h4>

<p>
  A natureza da representação define como a imagem é tratada pelo computador:
</p>

<ul>
  <li>
    <strong>Imagens Vetoriais:</strong> Descrições sintéticas baseadas inteiramente
    em equações e funções. Podem incluir atributos de cor e transparência e não perdem
    resolução ao serem redimensionadas.
  </li>
  <li>
    <strong>Imagens Digitais:</strong> São fotografias ou versões digitalizadas (pixeladas)
    de imagens vetoriais, representando a cena como um conjunto fixo de dados em
    vez de fórmulas matemáticas.
  </li>
</ul>

<h3>Imagem Matricial e Digitalização</h3>

<p>
  A imagem matricial é a forma como o computador organiza visualmente dados
  numéricos em uma grade bidimensional, transformando funções matemáticas em
  elementos visíveis.
</p>

<h4>Do Cálculo à Matriz</h4>

<p>Uma função discreta f(x, y) pode ser convertida em uma matriz onde:</p>

<ul>
  <li><strong>Colunas:</strong> Representam a coordenada x.</li>
  <li><strong>Linhas:</strong> Representam a coordenada y.</li>
  <li>
    <strong>Valores da Matriz:</strong> Representam a cor ou tom. Em uma escala de
    cinza simples, o valor 0 representa o preto e o valor 255 representa o branco.
  </li>
</ul>

<h4>Definições e Formatos</h4>

<ul>
  <li>
    <strong>Pixel:</strong> É a menor unidade de uma imagem digital (aglutinação
    de picture element).
  </li>
  <li>
    <strong>Imagem Digital (Raster ou Bitmap):</strong> É a imagem composta por essa
    grade de pixels.
  </li>
  <li>
    <strong>Armazenamento:</strong>
    <ul>
      <li>
        <strong>Sem compressão:</strong> Formatos como BMP salvam todos os pixels
        individualmente, gerando arquivos grandes.
      </li>
      <li>
        <strong>Com compressão:</strong> Formatos como JPEG, PNG ou TIFF utilizam
        algoritmos para reduzir o tamanho do arquivo.
      </li>
    </ul>
  </li>
</ul>

<h4>Organização da Memória (Padrão Raster)</h4>

<p>
  Embora vejamos a imagem como uma grade (2D), o computador a armazena na
  memória como um <strong>vetor unidimensional</strong> de bytes. Para localizar
  um pixel específico na linha <strong>L</strong> e coluna <strong>C</strong>,
  utiliza-se o cálculo:
</p>

<ul>
  <li>
    <strong>Posição = L * W + C</strong> (onde <strong>W</strong> é a largura ou
    tamanho de cada linha).
  </li>
</ul>

<p>
  A leitura ocorre sequencialmente: primeiro todos os elementos da linha 0,
  depois os da linha 1, e assim por diante.
</p>

<h4>Vetorial vs. Matricial no Uso Prático</h4>

<ul>
  <li>
    <strong>Arquivos Vetoriais (SVG, CDR, DWG):</strong> Armazenam apenas os "descritores"
    (as fórmulas das formas).
  </li>
  <li>
    <strong>Exibição:</strong> Para que uma imagem vetorial apareça na tela, o software
    precisa realizar a digitalização integral, lendo os descritores e desenhando
    cada forma para gerar uma imagem digital (pixels) em tempo real.
  </li>
</ul>

<h3>Conclusão</h3>

<p>
  Os conceitos-chave do que foram vistos nesta abordagem tratam daquilo que deve
  ficar mais claro, embora todos os pontos vistos, ao longo da exposição, sejam
  importantes para o entendimento do conteúdo. Iniciamos este conteúdo
  discutindo os passos necessários para iniciar na computação gráfica, passando
  por aspectos de pré-requisitos de hardware até softwares dedicados.
</p>

<p>
  Na sequência, procuramos explorar sobre o que trata a computação gráfica,
  contextualizando uma série de termos técnicos específicos. Esses termos serão
  muito usados nos conteúdos seguintes, em especial quando trabalharmos em áreas
  específicas. Falando no assunto, desmembramos, na sequência, as subáreas da
  computação gráfica, discutindo aspectos específicos da modelagem
  tridimensional, da síntese de imagens, da visão computacional e do
  processamento de imagens. Separamos também quais elementos básicos da
  computação são englobados por cada ramo específico.
</p>

<p>
  Posteriormente, discutimos os primeiros aspectos da geometria da construção de
  imagens, em especial as formas bidimensionais das retas e cônicas, além das
  funções matemáticas. Finalmente, antes do encerrarmos esta abordagem,
  observamos as principais propriedades das imagens matriciais, discutindo as
  diferenças das mesmas com as imagens vetoriais, além da possibilidade de
  compactação das mesmas com algoritmos especializados.
</p>
