<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Matrizes na Computação Gráfica</h2>

<Audios modulo="M7" aulas={["05", "06", "07", "08"]} />

<p>
  As transformações geométricas em computação gráfica são implementadas por meio
  de cálculos matriciais. A complexidade e o volume desses cálculos justificam a
  necessidade de placas de vídeo (GPUs) dedicadas, que são otimizadas para
  processar essas estruturas simultaneamente.
</p>

<p>
  Uma matriz é uma estrutura bidimensional composta por elementos do mesmo tipo,
  organizados em linhas e colunas. Cada elemento é identificado por sua posição
  específica e seu valor. Existem formatos específicos que recebem nomenclaturas
  distintas:
</p>

<ul>
  <li>
    <strong>Matriz Genérica:</strong> Identificada pelo número de linhas e colunas
    (ex: uma matriz 2 X 3 possui duas linhas e três colunas).
  </li>
  <li>
    <strong>Vetor:</strong> Uma matriz que possui apenas uma linha ou apenas uma
    coluna.
  </li>
  <li>
    <strong>Matriz Quadrada:</strong> Estrutura que possui o mesmo número de linhas
    e colunas.
  </li>
  <li>
    <strong>Matriz Identidade:</strong> Uma matriz quadrada que funciona como o número
    1 nas operações matriciais, servindo como elemento neutro.
  </li>
</ul>

<h3>Operações com Matrizes</h3>

<p>
  As operações básicas de matrizes formam a lógica por trás da manipulação de
  objetos no espaço digital. Abaixo, as principais operações e suas regras:
</p>

<h4>Soma e Subtração</h4>

<p>
  Estas operações só podem ser realizadas entre matrizes de <strong
    >mesma dimensão</strong
  >
  (mesmo número de linhas e colunas). O cálculo é feito elemento a elemento: o valor
  na posição a<sub>11</sub> da primeira matriz soma-se ou subtrai-se ao valor na
  posição b<sub>11</sub> da segunda, e assim sucessivamente.
</p>

<h4>Matriz Transposta</h4>

<p>
  A transposição consiste na troca sistemática de linhas por colunas. Se uma
  matriz possui uma linha com os valores x e y, na sua transposta esses valores
  formarão a coluna (x, y)<sup>T</sup>. Um caso particular é a
  <strong> matriz identidade </strong>, cuja transposta é igual a ela mesma.
</p>

<h4>Multiplicação de Matrizes</h4>

<p>
  Diferente da soma, a multiplicação exige que o <strong>
    número de colunas da primeira matriz seja igual ao número de linhas da
    segunda
  </strong>. O resultado será uma matriz com o número de linhas da primeira e o
  número de colunas da segunda.
</p>

<ul>
  <li>
    Procedimento: Os elementos da matriz resultante são obtidos pela soma dos
    produtos dos elementos da linha da primeira matriz pelos elementos
    correspondentes da coluna da segunda.
  </li>
  <li>
    Exemplo de Dimensão: Se multiplicarmos uma matriz 2 X 3 por uma 3 X 2, o
    resultado será uma matriz quadrada 2 X 2.
  </li>
</ul>

<h3>Transformações Geométricas</h3>

<p>
  A posição de um ponto com coordenadas x e y pode ser representada pela matriz
  coluna (x, y)<sup>T</sup>. Essa representação facilita o cálculo de
  transformações através de operações matriciais.
</p>

<p>
  Uma transformação de um ponto P é realizada multiplicando-o por uma matriz de
  transformação T, resultando em um novo ponto P'. A operação é expressa por P'
  = T . P. Para reverter uma transformação e voltar ao estado original,
  aplica-se a matriz inversa: P = T<sup>-1</sup> . P'.
</p>

<h4>Aplicação em 2D e 3D</h4>

<p>
  As transformações funcionam de forma análoga tanto no plano quanto no espaço,
  alterando apenas a dimensão das matrizes:
</p>

<ul>
  <li>
    <strong>No plano (2D):</strong> O ponto (x, y)<sup>T</sup> é transformado pela
    matriz para gerar as novas coordenadas.
  </li>
  <li>
    <strong>No espaço (3D):</strong> Utiliza-se a mesma lógica matricial, porém
    com um vetor de três componentes, como (u, v, w)<sup>T</sup>, para
    representar a profundidade e evitar confusão com o sistema bidimensional.
  </li>
</ul>

<h3>Translação</h3>

<p>
  A animação gráfica e a manipulação de janelas ou personagens baseiam-se em
  transformações geométricas. A <strong>translação</strong> consiste em deslocar
  um objeto somando valores específicos às suas coordenadas originais. Por
  exemplo, para mover um ponto para a direita e para cima, somamos valores aos
  eixos <strong>x e y</strong>.
</p>

<p>
  Para realizar essa operação através de uma <strong
    >multiplicação de matrizes</strong
  >
  (padronizando o processo com outras transformações), utiliza-se uma dimensão extra.
  Em um sistema 2D, trabalhamos com uma matriz 3 x 3 e um ponto representado por
  (x, y, 1)<sup>P</sup>.
</p>

<ul>
  <li>
    <strong>No plano (2D):</strong> Para deslocar um ponto até (x', y')<sup
      >T</sup
    >, utiliza-se uma matriz de translação que contém os valores de deslocamento
    t<sub>x</sub>
    e t<sub>y</sub>.
  </li>
  <li>
    <strong>No espaço (3D):</strong> A lógica é idêntica, mas utiliza-se uma
    matriz 4 x 4 para comportar os deslocamentos nos três eixos: t<sub>x</sub>,
    t<sub>y</sub> e t<sub>z</sub>, aplicados ao ponto (x, y, z, 1)<sup>T</sup>.
  </li>
</ul>

<h4>Escala</h4>

<p>
  A alteração de escala consiste em redimensionar um objeto, aumentando ou
  diminuindo seu tamanho. Isso é feito multiplicando cada coordenada por um
  fator de escala.
</p>

<ul>
  <li>Se o fator for maior que 1, o objeto aumenta.</li>
  <li>Se o fator estiver entre 0 e 1, o objeto diminui.</li>
</ul>

<p>
  Assim como na translação, a escala é aplicada através de uma matriz de
  transformação onde os fatores de escala (s<sub>x</sub>, s<sub>y</sub>, s<sub
    >z</sub
  >) ocupam a diagonal principal da matriz.
</p>

<p>
  A alteração de escala consiste em redimensionar um objeto, alterando a
  distância entre seus pontos. Para isso, multiplicamos as coordenadas originais
  por fatores de escala.
</p>

<ul>
  <li>
    <strong>Ampliação:</strong> Ocorre quando os fatores são maiores que 1.
  </li>
  <li>
    <strong>Redução:</strong> Ocorre quando os fatores estão no intervalo entre 0
    e 1.
  </li>
</ul>

<h4>Representação Matricial</h4>

<p>
  Em duas dimensões, os fatores s<sub>x</sub> e s<sub>y</sub> definem quanto o objeto
  será ampliado ou reduzido em cada eixo. A operação é dada por P' = S . P, onde
  a matriz de escala S posiciona os fatores na diagonal principal.
</p>

<ul>
  <li>
    No plano (2D): Utiliza-se uma matriz 3 x 3 para manter a compatibilidade com
    a dimensão extra da translação. O ponto é representado por (x, y, 1)<sup
      >T</sup
    >.
  </li>
  <li>
    No espaço (3D): Utiliza-se uma matriz 4 x 4 com fatores s<sub>x</sub>, s<sub
      >y</sub
    >
    e s<sub>z</sub> para os três eixos, aplicada ao ponto (x, y, z, 1)<sup
      >T</sup
    >.
  </li>
</ul>

<h4>Exemplo Prático (Triângulo)</h4>

<p>Considere um triângulo com vértice em A = (1, 1, 1)<sup>T</sup>:</p>

<ol>
  <li>
    <strong>Translação:</strong> Para mover 3 unidades à direita (t<sub>x</sub>
    = 3) e 2 para cima (t<sub>y</sub> = 2), a matriz de translação transforma o
    ponto A no ponto A' = (4, 3, 1)<sup>T</sup>.
  </li>
  <li>
    <strong>Escala:</strong> Para ampliar o triângulo em 2 vezes no eixo x (s<sub
      >x</sub
    >
    = 2) e 3 vezes no eixo y (s<sub>y</sub> = 3), a matriz de escala transforma
    o ponto A no ponto A'' = (2, 3, 1)<sup>T</sup>.
  </li>
</ol>

<h3>Rotação e Reflexão</h3>

<p>
  Além da translação e escala, a <strong>rotação</strong> e a
  <strong>reflexão</strong> completam o conjunto principal de transformações geométricas.
</p>

<h4>Rotação</h4>

<p>
  Consiste no "giro" de um ponto em torno de uma origem. Em duas dimensões, o
  sentido padrão é o anti-horário. A matriz de rotação utiliza funções
  trigonométricas (<strong>sen</strong> e <strong>cos</strong>) para calcular as
  novas coordenadas.
</p>

<ul>
  <li>
    <strong>No plano (2D):</strong> A rotação por um ângulo θ transforma o ponto
    (x, y, 1)<sup>T</sup> através de uma matriz que combina cossenos e senos.
  </li>
  <li>
    <strong>No espaço (3D):</strong> A rotação ocorre em torno de um eixo específico
    (x, y ou z). Por exemplo, em uma rotação em torno do eixo z, as coordenadas x
    e y mudam, enquanto a coordenada z permanece constante.
  </li>
</ul>

<h4>Reflexão</h4>

<p>
  Funciona como um espelho, invertendo a posição do objeto em relação a um eixo
  ou plano. Na prática, isso é feito negativando uma das coordenadas.
</p>

<ul>
  <li><strong>Eixo x:</strong> Inverte o sinal de y.</li>
  <li><strong>Eixo y:</strong> Inverte o sinal de x.</li>
  <li>
    <strong>Em 3D:</strong> A inversão ocorre em relação aos planos (xy, xz ou yz).
    Por exemplo, refletir no plano xy inverte o sinal da coordenada z.
  </li>
</ul>

<h4>Concatenação e Comutatividade</h4>

<p>
  Uma das maiores vantagens do uso de matrizes é a capacidade de combinar várias
  transformações (ex: rotacionar e depois transladar) em uma única <strong>
    matriz composta
  </strong>, bastando multiplicar as matrizes originais. No entanto, é preciso
  atenção a dois pontos:
</p>

<ol>
  <li>
    <strong>Não Comutatividade:</strong> A ordem das operações importa.
    Multiplicar a matriz de <strong>Rotação</strong> pela de
    <strong>Translação</strong>
    geralmente resulta em algo diferente de
    <strong>Translação</strong> por <strong>Rotação</strong>.
  </li>
  <li>
    <strong>Posicionamento:</strong> As matrizes apresentadas exigem que o ponto
    (x, y, 1)<sup>T</sup> esteja à direita da matriz de transformação. Caso o ponto
    seja representado como matriz linha, deve-se utilizar a transposta da matriz
    de transformação.
  </li>
</ol>

<p>
  <strong>Exemplo Prático:</strong> Para rotacionar o ponto A = (3, 2, 1)<sup
    >T</sup
  >
  em 90°, aplicamos os valores de cos(90°) = 0 e sen(90°) = 1 na matriz, resultando
  no novo ponto A' = (-2, 3, 1)<sup>T</sup>.
</p>

<h3>Conclusão</h3>

<p>
  A computação gráfica utiliza o formalismo das matrizes para processar imagens
  e modelos. A eficiência das GPUs deve-se à sua capacidade de realizar esses
  cálculos matemáticos de forma massiva e paralela.
</p>

<ol>
  <li>
    <strong>Estruturas e Operações Essenciais</strong>
    <ul>
      <li>
        <strong>Matrizes e Vetores:</strong> Pontos no espaço são tratados como
        vetores coluna na forma (x, y, 1)<sup>T</sup> (para 2D) ou (x, y, z, 1)<sup
          >T</sup
        > (para 3D).
      </li>
      <li>
        <strong>Multiplicação:</strong> É a operação vital para transformações. O
        número de colunas da primeira matriz deve ser igual ao de linhas da segunda.
      </li>
      <li>
        <strong>Transposição:</strong> Inversão de linhas por colunas, essencial
        quando mudamos a forma de representar o ponto (de coluna para linha).
      </li>
    </ul>
  </li>
  <li>
    <strong>Transformações Geométricas Principais</strong>
    <ul>
      <li>
        <strong>Translação:</strong> Desloca o objeto somando valores aos eixos.
        Requer uma dimensão extra (coordenadas homogêneas) para ser executada via
        multiplicação.
      </li>
      <li>
        <strong>Escala:</strong> Multiplica as coordenadas por fatores s<sub
          >x</sub
        >, s<sub>y</sub>, s<sub>z</sub>. Valores &gt; 1 ampliam; entre 0 e 1
        reduzem.
      </li>
      <li>
        <strong>Rotação:</strong> Gira o objeto em torno da origem (2D) ou de eixos
        específicos (3D) usando funções de seno e cosseno.
      </li>
      <li>
        <strong>Reflexão:</strong> Inverte o objeto como um espelho ao negativar
        coordenadas em relação a um eixo ou plano.
      </li>
    </ul>
  </li>
  <li>
    <strong>Matrizes Compostas</strong>
    <ul>
      <li>
        As transformações podem ser "empilhadas". Podemos criar uma única <strong
        >
          Matriz de Transformação Composta
        </strong> multiplicando as matrizes de escala, rotação e translação.
      </li>
      <li>
        <strong>Atenção:</strong> A ordem importa! Como a multiplicação de matrizes
        não é comutativa, o resultado de "rotacionar e depois mover" é diferente
        de "mover e depois rotacionar".
      </li>
    </ul>
  </li>
</ol>
