<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Estruturas de Programação</h2>

<Audios modulo="M3" aulas={["05", "06", "07", "08"]} />

<h3>Introdução</h3>

<p>
  Este conteúdo aborda a nomeação de estruturas, declaração de variáveis, tipos
  de dados e matrizes, com foco em compreender a aplicação de identificadores e
  o uso de estruturas de dados.
</p>

<h4>Nomes (Identificadores)</h4>

<p>
  Na programação, nomes ou identificadores são cadeias de caracteres usadas para
  identificar entidades no código, permitindo localizar sentenças e variáveis
  posteriormente. Para evitar problemas de sintaxe, a construção de
  identificadores segue regras comuns à maioria das linguagens:
</p>

<ul>
  <li><strong>Início:</strong> Deve começar obrigatoriamente com uma letra.</li>
  <li>
    <strong>Continuação:</strong> Pode ser seguido por letras ou dígitos numéricos.
  </li>
  <li><strong>Espaçamento:</strong> É proibido o uso de espaços em branco.</li>
  <li>
    <strong>Conectores:</strong> O sublinhado (_, underscore) pode ser utilizado
    para separar palavras.
  </li>
</ul>

<p>
  Existem também padrões de escrita para unir palavras consecutivas sem espaços:
</p>

<ul>
  <li>
    <strong>PascalCase:</strong> Une as palavras iniciando todas com a primeira letra
    maiúscula.
  </li>
  <li>
    <strong>camelCase:</strong> Semelhante ao PascalCase, mas a primeira letra da
    primeira palavra permanece minúscula.
  </li>
</ul>

<h4>Sensibilidade a Maiúsculas e Minúsculas (Case Sensitivity)</h4>

<p>
  Linguagens baseadas em C são case-sensitives, o que significa que diferenciam
  letras maiúsculas de minúsculas. Sob essa regra, Var1 e var1 são tratados como
  dois identificadores distintos.
</p>

<p>
  <strong>Convenção:</strong> Para evitar erros, adota-se a prática comum de escrever
  variáveis sempre com letras minúsculas.
</p>

<h4>Caracteres Especiais de Identificação</h4>

<p>
  Algumas linguagens de programação exigem o uso de caracteres iniciais
  específicos para categorizar e diferenciar seus elementos:
</p>

<ul>
  <li><strong>PHP:</strong> Variáveis iniciam com $.</li>
  <li><strong>Perl:</strong> Elementos iniciam com $, @ ou %.</li>
  <li><strong>Ruby:</strong> Utiliza-se @ ou @@ em situações específicas.</li>
</ul>

<h3>Palavras Especiais e Variáveis</h3>

<h4>Palavras Especiais</h4>

<p>
  As palavras especiais servem para nomear ações específicas e aumentar a
  legibilidade dos programas. Elas são divididas em duas categorias:
</p>

<ul>
  <li>
    <strong>Palavras-chave:</strong> Palavras que são especiais apenas em determinados
    contextos. Seu uso atualmente é muito restrito, limitando-se basicamente ao Fortran.
  </li>
  <li>
    <strong>Palavras reservadas:</strong> Termos de uso específico que não podem
    ser utilizados como identificadores sob nenhuma circunstância.
  </li>
  <li>
    <strong>Nota:</strong> Quanto maior o número de palavras reservadas em uma linguagem,
    mais complexa se torna a criação de identificadores, pois aumenta o risco de
    colisões sintáticas.
  </li>
</ul>

<h4>Variáveis</h4>

<p>
  Uma variável é a abstração de uma célula ou de um conjunto de células de
  memória do computador. Os identificadores substituem os endereços hexadecimais
  nativos da memória (como 0xA2 ou 0x11) para facilitar a manipulação dos dados.
</p>

<h4>Atributos de uma Variável</h4>

<p>As variáveis são caracterizadas por seis atributos essenciais:</p>

<ul>
  <li>
    <strong>Nome:</strong> O identificador escolhido para batizá-la no código.
  </li>
  <li>
    <strong>Endereço (l-value):</strong> O local físico mapeado na memória. Quando
    nomes diferentes apontam para o mesmo endereço, ocorre o fenômeno do apelido
    (alias).
  </li>
  <li>
    <strong>Valor (r-value):</strong> O conteúdo armazenado no endereço de memória.
  </li>
  <li>
    <strong>Tipo:</strong> Determina a faixa de valores que a variável pode armazenar
    (inteiros, decimais, caracteres, booleanos) e as operações permitidas.
  </li>
  <li>
    <strong>Tempo de vida:</strong> O período de tempo em que a variável permanece
    vinculada a uma posição de memória.
  </li>
  <li>
    <strong>Escopo:</strong> A região do programa onde a variável é visível e pode
    ser acessada.
  </li>
</ul>

<h4>Classificação quanto à Permanência na Memória</h4>

<ul>
  <li>
    <strong>Estáticas:</strong> Permanecem vinculadas à mesma posição de memória
    durante toda a execução do programa.
  </li>
  <li>
    <strong>Dinâmicas da pilha:</strong> Criadas e vinculadas diretamente no momento
    de sua declaração.
  </li>
  <li>
    <strong>Dinâmicas do monte explícitas:</strong> Alocadas e desalocadas por meio
    de instruções explícitas no código.
  </li>
  <li>
    <strong>Dinâmicas do monte implícitas:</strong> Vinculadas apenas no momento
    da atribuição de valores.
  </li>
</ul>

<h4>Escopos e Blocos</h4>

<ul>
  <li>
    <strong>Escopo:</strong> Termo geral para definir um trecho do programa. O escopo
    estático abrange qualquer seção determinada estaticamente antes da execução do
    código.
  </li>
  <li>
    <strong>Blocos:</strong> São escopos estáticos restritos definidos diretamente
    na escrita do código que possuem suas próprias variáveis locais. Em linguagens
    baseadas em C, são delimitados por chaves &lbrace; &rbrace;.
  </li>
  <li>
    <strong>Blocos aninhados:</strong> Estruturas onde um bloco é inserido dentro
    de outro.
  </li>
  <li>
    <strong>Ambiente de referenciamento:</strong> O conjunto de todas as variáveis
    visíveis em um determinado bloco.
  </li>
  <li>
    <strong>Nota de Sintaxe:</strong> A posição da abertura das chaves (na mesma
    linha da instrução ou na linha seguinte) não altera a compilação ou o funcionamento
    do programa em linguagens baseadas em C; a escolha é puramente estilística ou
    didática.
  </li>
</ul>

<h4>Constantes Nomeadas</h4>

<p>
  Uma constante nomeada é um identificador vinculado a um valor fixo que não
  pode ser alterado durante a execução do programa. O seu uso melhora a
  legibilidade e a confiabilidade do código. Em C++, uma constante é declarada
  utilizando a palavra reservada const:
</p>

<code>
  <pre>
  const int horas = 24;
  </pre>
</code>

<p>
  Algumas linguagens voltadas para computação científica (como o MATLAB) já
  possuem constantes predefinidas em seu ambiente, como pi = 3.14159.
</p>

<h3>Tipos de Dados</h3>

<p>
  O tipo de dado define o conjunto de valores possíveis que uma estrutura pode
  assumir e todas as operações que podem ser realizadas com eles. Os dados
  inseridos no código devem corresponder à natureza das informações no mundo
  real.
</p>

<h4>Particionamento de Memória</h4>

<p>
  A organização do espaço de armazenamento no computador utiliza terminologias
  específicas para o agrupamento de dados binários:
</p>

<ul>
  <li>
    <strong>Bit (Binary Digit):</strong> A unidade mínima de informação, assumindo
    os valores 0 ou 1. Na programação de alto nível, bits individuais funcionam principalmente
    como flags (sinalizadores de eventos ou estados).
  </li>
  <li><strong>Nibble:</strong> Agrupamento de 4 bits.</li>
  <li><strong>Byte (ou Octeto):</strong> Agrupamento de 8 bits.</li>
  <li>
    <strong>Word:</strong> Agrupamento de 16 bits (equivalente a 2 bytes).
  </li>
</ul>

<h4>Tipos de Dados Primitivos</h4>

<p>
  Os tipos primitivos são aqueles nativos da linguagem, não definidos em termos
  de outros tipos de dados.
</p>

<h4>Inteiro</h4>

<p>
  Armazena valores numéricos positivos ou negativos sem parte fracionária. É
  frequentemente utilizado para contagens. A maioria das linguagens oferece
  quatro tamanhos padrão baseados no número de bits:
</p>

<ul>
  <li><strong>Byte:</strong> 8 bits</li>
  <li>
    <strong>Short:</strong> 16 bits (armazena $2^&lbrace;16&rbrace; = 65.536$ valores
    diferentes; tipicamente de -32.768 a 32.768, usando o bit mais à esquerda para
    o sinal)
  </li>
  <li><strong>Int:</strong> 32 bits</li>
  <li><strong>Long:</strong> 64 bits</li>
</ul>

<h4>Exemplos de declaração em C++:</h4>

<code>
  <pre>
  int nomeDaVariavel;
  int var1 = 50
  </pre>
</code>

<h4>Ponto Flutuante (Floating Point)</h4>

<p>
  Modela números reais armazenando seus algarismos significativos. Funciona de
  forma análoga à notação científica ($\pm m \times 10^n$), dividindo a
  estrutura de bits em sinal, expoente (ordem de grandeza com base 2) e fração
  (mantissa).Na programação, a escrita adota o ponto decimal e a letra E ou e
  para representar a potência de base 10 (ex: $132.000.000 = 1,32 \times 10^8$ é
  escrito como 1.32E8 ou 1.32e8).Devido à limitação de bits, os valores são
  aproximados e podem sofrer perda de precisão. Para mitigar isso, existem duas
  variações de tamanho:
</p>

<ul>
  <li><strong>Float:</strong> 32 bits.</li>
  <li>
    <strong>Double:</strong> 64 bits (oferece maior precisão e maior largura de expoentes).
  </li>
</ul>

<h4>Exemplos de declaração em C++:</h4>

<code>
  <pre>
  float nomeDaVariavel;
  float valor = 7.5e3; // Declaração correta de tipo real com atribuição de 7,5
    x 10³
  </pre>
</code>

<h4>Outros Tipos Numéricos</h4>

<ul>
  <li>
    <strong>Complexos:</strong> Pares ordenados de ponto flutuante com operações
    aritméticas próprias, suportados nativamente por linguagens como Fortran e Python.
  </li>
  <li>
    <strong>Decimais:</strong> Voltados para sistemas de negócios em computadores
    de grande porte. Armazenam uma quantidade grande e fixa de casas decimais de
    forma precisa, porém possuem faixa de valores restrita e alto consumo de memória.
  </li>
</ul>

<h3>Declaração de Dados</h3>

<h4>Dados Booleanos</h4>

<p>
  O tipo booleano é o dado que ocupa o menor espaço na memória, necessitando
  logicamente de apenas um único bit. No entanto, devido às restrições de
  endereçamento dos computadores, é comum utilizar um byte completo para o seu
  armazenamento.
</p>

<ul>
  <li><strong>Valores possíveis:</strong> 0 ou 1.</li>
  <li>
    <strong>Representação no código:</strong> Manipulado por meio de atribuições
    lógicas escritas obrigatoriamente em letras minúsculas: true (verdadeiro, equivalente
    a 1) e false (falso, equivalente a 0).
  </li>
</ul>

<h4>Exemplos de declaração em C++:</h4>

<code>
  <pre>
  bool nomeDaVariavel;
  bool estado = true;
  </pre>
</code>

<h4>Caracteres</h4>

<p>
  Os caracteres armazenam letras, símbolos ou dígitos isolados por meio de uma
  codificação numérica padronizada.
</p>

<ul>
  <li>
    <strong>Padrão ASCII:</strong> É o modelo mais antigo e amplamente utilizado.
    Consome 8 bits de espaço, mas define apenas 128 caracteres indexados, utilizando
    efetivamente 7 bits para a codificação (o bit mais à esquerda assume funções
    variadas dependendo do contexto).
  </li>
  <li>
    <strong>Padrão Unicode:</strong> Modelo mais moderno que utiliza 16 bits, abrangendo
    caracteres da maioria das linguagens naturais do mundo.
  </li>
</ul>

<p>
  Na sintaxe do código, os valores do tipo caractere devem ser delimitados por
  aspas simples (' ') para diferenciá-los dos identificadores de variáveis.
</p>

<h4>Exemplos de declaração em C++:</h4>

<code>
  <pre>
  char nomeDoCaractere;
  char item = 'a';
  </pre>
</code>

<h4>Cadeia de Caracteres (Strings)</h4>

<p>
  A cadeia de caracteres consiste em uma sequência ou conjunto consecutivo de
  caracteres. Em linguagens como C e C++, sua declaração e implementação
  estrutural ocorrem por meio de vetores de caracteres (char).
</p>

<h3>Matrizes</h3>

<p>
  A matriz é um agregado homogêneo de elementos de dados, onde cada elemento
  individual é identificado por sua posição.
</p>

<h4>Identificação e Acesso</h4>

<p>
  Os elementos de uma matriz são indicados pelo nome da estrutura seguido de
  índices, geralmente envoltos em colchetes [ ].
</p>

<ul>
  <li>
    <strong>Convenção de colchetes:</strong> O uso de colchetes é predominante para
    evitar confusões com funções, que utilizam parênteses.
  </li>
  <li>
    <strong>Exceções:</strong> Fortran e Ada utilizam parênteses. Em Perl, as matrizes
    são identificadas pelo caractere inicial @, enquanto variáveis escalares usam
    $.
  </li>
  <li>
    <strong>Indexação:</strong> A contagem das posições dos elementos inicia-se obrigatoriamente
    a partir do zero 0.
  </li>
</ul>

<h4>Declaração em Linguagens Baseadas em C</h4>

<p>
  As matrizes devem ser declaradas no início do programa ou em sua primeira
  utilização. A atribuição de valores iniciais não é obrigatória no momento da
  declaração.
</p>

<h4>Matrizes Unidimensionais (Vetores)</h4>

<p>Possuem apenas uma dimensão.</p>

<code>
  <pre>
  // Declaração com atribuição de valores
  int nomeDaMatriz [4] = &lbrace;10, 20, 30, 40&rbrace;;
  // Declaração sem atribuição
  int coordenadas [3];
  </pre>
</code>

<h4>Matrizes Multidimensionais</h4>

<p>
  Para estruturas com mais dimensões, acrescentam-se colchetes extras para cada
  dimensão. Em uma matriz bidimensional de dimensão $3 \times 2$ (3 linhas e 2
  colunas):
</p>

<code>
  <pre>
  int mat1 [3][2];
  </pre>
</code>

<p>
  Os elementos dessa matriz são acessados individualmente pelas posições:
  mat1[0][0], mat1[0][1], mat1[1][0], mat1[1][1], mat1[2][0] e mat1[2][1].
</p>

<h4>Cadeia de Caracteres (Strings)</h4>

<p>
  Em C ou C++, uma string pode ser declarada estruturalmente como uma matriz de
  caracteres:
</p>

<code>
  <pre>
  char nomeDoVetor [5] = "valor";
  </pre>
</code>

<h4>Operações e Termos Específicos</h4>

<p>
  Na maioria das linguagens de programação, as operações algébricas (soma,
  subtração, produto, inversa e transposta) não são realizadas de forma direta
  entre as matrizes. Essas operações exigem codificação manual ou o uso de
  métodos específicos fornecidos por linguagens como Java, C++ ou C#.
</p>

<h4>Termos Relacionados:</h4>

<ul>
  <li>
    <strong>Matriz retangular:</strong> Possui todas as linhas com o mesmo número
    de elementos.
  </li>
  <li>
    <strong>Matriz irregular:</strong> Apresenta linhas com tamanhos (quantidade
    de elementos) diferentes.
  </li>
  <li>
    <strong>Fatica (Slice):</strong> Uma subestrutura extraída de uma matriz.
  </li>
  <li>
    <strong>Registros:</strong> Estruturas semelhantes às matrizes, porém compostas
    por dados de diferentes tipos e/ou tamanhos.
  </li>
  <li>
    <strong>União:</strong> Variáveis que podem armazenar diferentes tipos de valores
    em momentos distintos da execução do programa.
  </li>
</ul>

<h4>Exemplos Práticos de Matrizes Bidimensionais em C++</h4>

<ul>
  <li>
    <strong>Matriz de Inteiros (3 x 3):</strong>
    <pre>
      int A[3][3] = &lbrace;&lbrace;11, 12, 13&rbrace;, &lbrace;21, 22, 23&rbrace;, &lbrace;31, 32, 33&rbrace;&rbrace;;
    </pre>
  </li>
  <li>
    <strong>Matriz de Reais (2 x 2):</strong>
    <pre>
      float B[2][2] = &lbrace;&lbrace;6.5, 7.2&rbrace;, &lbrace;4.3, 5.5&rbrace;&rbrace;;
    </pre>
    <ul>
      <li>
        <strong>Exemplo de Acesso:</strong> Para isolar e acessar especificamente
        o valor 7.2 contido na matriz B, referencia-se a primeira linha (índice 0)
        e a segunda coluna (índice 1): B[0][1].
      </li>
    </ul>
  </li>
</ul>

<h3>Conclusão: Conceitos-Chave</h3>

<p>
  Este fechamento recapitula os fundamentos essenciais abordados na etapa sobre
  estruturas de dados e identificadores.
</p>

<h4>Identificadores e Palavras Especiais</h4>

<ul>
  <li>
    <strong>Regras de Nomeação:</strong> Os nomes de variáveis e demais estruturas
    devem iniciar obrigatoriamente com letras, podendo ser seguidos por números e
    sublinhados (_).
  </li>
  <li>
    <strong>Sintaxe Específica:</strong> Cada linguagem possui exigências próprias
    para a expressão de nomes, demandando atenção às suas regras de construção.
  </li>
  <li>
    <strong>Restrições:</strong> É fundamental identificar e evitar o uso de palavras
    especiais da linguagem ao nomear os elementos do código.
  </li>
</ul>

<h4>Armazenamento e Variáveis</h4>

<ul>
  <li>
    <strong>Natureza:</strong> As variáveis funcionam como posições organizadas dentro
    da memória do computador para o armazenamento de dados.
  </li>
  <li>
    <strong>Temporalidade e Escopo:</strong> O tempo de permanência de um dado na
    memória varia conforme a classificação da variável, que pode ser válida apenas
    dentro de blocos específicos ou por todo o programa.
  </li>
  <li>
    <strong>Diversidade de Tipos:</strong> A memória gerencia dados de diferentes
    tamanhos e aplicações práticas, destacando-se os tipos inteiros, booleanos e
    caracteres.
  </li>
</ul>

<h4>Matrizes</h4>

<ul>
  <li>
    <strong>Agrupamento:</strong> As matrizes consistem em coleções de dados estruturadas
    de forma homogênea para facilitar a manipulação conjunta.
  </li>
  <li>
    <strong>Sintaxe:</strong> A correta aplicação das matrizes exige o cumprimento
    estrito das regras de declaração e preenchimento de índices definidas pela linguagem
    de programação.
  </li>
</ul>
