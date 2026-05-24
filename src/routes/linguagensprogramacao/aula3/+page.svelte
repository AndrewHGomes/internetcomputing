<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Expressões</h2>

<Audios modulo="M3" aulas={["09", "10", "11", "12"]} />

<h3>Introdução e Objetivos</h3>

<p>
  Esta etapa do conteúdo formaliza os conceitos de operações algébricas e
  booleanas no contexto da programação. O objetivo principal é compreender como
  o computador realiza esses cálculos de forma precisa e rápida. Os tópicos
  abordados são:
</p>

<ul>
  <li>Expressões</li>
  <li>Operações algébricas</li>
  <li>Conversões de tipos e sentenças de atribuição</li>
  <li>Operadores relacionais</li>
  <li>Álgebra booleana</li>
</ul>

<h3>Expressões</h3>

<p>
  As expressões são os meios fundamentais para transcrever computações em uma
  linguagem de programação. Nelas, a ordem de avaliação dos operadores e dos
  operandos é um fator importante. As expressões aritméticas são compostas por:
</p>

<ul>
  <li>Operadores</li>
  <li>Operandos</li>
  <li>Parênteses</li>
  <li>Funções</li>
</ul>

<h4>Tipos de Operadores quanto aos Operandos</h4>

<ul>
  <li><strong>Unários:</strong> Possuem apenas um operando.</li>
  <li><strong>Binários:</strong> Possuem dois operandos.</li>
  <li><strong>Ternários:</strong> Necessitam de três operandos.</li>
</ul>

<h4>Notações de Ordenação</h4>

<ul>
  <li>
    <strong>Infix (Notação convencional):</strong> O operador é posicionado entre
    os operandos.
  </li>
  <li>
    <strong>Prefix (Notação polonesa):</strong> O operador aparece antes dos operandos.
  </li>
</ul>

<h3>Operações Algébricas</h3>

<p>
  Os operadores básicos seguem uma lógica semelhante na maioria das linguagens
  de programação:
</p>

<ul>
  <li><strong>Adição:</strong> +</li>
  <li><strong>Subtração:</strong> -</li>
  <li><strong>Multiplicação:</strong> *</li>
  <li><strong>Divisão:</strong> /</li>
</ul>

<p>
  Existem também operações unárias comuns para alteração de valores em uma
  unidade:
</p>

<ul>
  <li><strong>Incremento (++):</strong> Soma uma unidade ao valor.</li>
  <li><strong>Decremento (--):</strong> Subtrai uma unidade do valor.</li>
</ul>

<h4>Operações Específicas</h4>

<ul>
  <li>
    <strong>Resto da divisão:</strong> Representado por % ou rem dependendo da linguagem.
    É o valor que sobra quando a divisão chega a um número menor que o divisor.
  </li>
  <li>
    <strong>Potência:</strong> Representada por ou ^ em algumas linguagens.
  </li>
  <li>
    <strong>Módulo (Valor absoluto):</strong> Frequentemente representado por abs.
  </li>
</ul>

<h4>Precedência e Associatividade</h4>

<strong>Precedência</strong>

<p>
  Determina qual operação é realizada primeiro na execução do programa. As
  linguagens adotam regras de prioridade para os operadores (como executar a
  multiplicação antes da adição), que variam conforme a tecnologia utilizada. Os
  operadores unários, de potência ou de incremento/decremento costumam ter maior
  prioridade do que os operadores binários de adição e subtração.
</p>

<strong>Associatividade</strong>

<p>
  Define a ordem de execução (da esquerda para a direita ou da direita para a
  esquerda) quando operadores possuem o mesmo nível de precedência.
</p>

<ul>
  <li>
    A maioria das linguagens processa operações básicas (como adição e
    multiplicação) da esquerda para a direita.
  </li>
  <li>
    Operações de potência () ou operadores unários frequentemente associam da
    direita para a esquerda.
  </li>
  <li>
    Existem exceções, como a linguagem APL (que avalia tudo da direita para a
    esquerda) e o operador em Ada, que é não associativo.
  </li>
</ul>

<strong>Uso de Parênteses</strong>

<p>
  Na programação, utilizam-se exclusivamente os parênteses () para forçar ou
  modificar a precedência e a associatividade das operações, mesmo de forma
  aninhada ((())). Não são utilizados colchetes ou chaves para esta finalidade.
</p>

<h4>Conceitos Adicionais</h4>

<ul>
  <li>
    <strong>Transparência Referencial:</strong> Ocorre quando duas expressões com
    o mesmo valor podem ser substituídas uma pela outra no programa sem alterar o
    seu comportamento.
  </li>
  <li>
    <strong>Sobrecarga de Operadores:</strong> Acontece quando um único operador
    possui mais de um propósito no código. Esse recurso prejudica a legibilidade
    e pode dificultar o diagnóstico de erros.
  </li>
</ul>

<h3>Conversões de Tipos</h3>

<p>
  A conversão de tipos consiste em mover um dado de um local na memória para
  outro com tamanho ou formato diferente. Divide-se em duas categorias:
</p>

<ul>
  <li>
    <strong>Conversão de Estreitamento:</strong> Converte um valor para um tipo com
    capacidade menor (ex: double para float em Java). Pode alterar a magnitude do
    valor se ele estiver fora da faixa do destino.
  </li>
  <li>
    <strong>Conversão de Alargamento:</strong> Converte um valor para um tipo com
    capacidade maior (ex: int para float em Java). É mais segura, mas pode causar
    perda de precisão nos bits finais.
  </li>
</ul>

<h4>Expressões de Modo Misto e Coerção</h4>

<p>
  Expressões de modo misto possuem operandos de tipos diferentes. Nelas, ocorre
  a coerção (conversão implícita), onde o sistema converte os tipos
  automaticamente, gerando menor controle para o programador. Para evitar isso,
  utilizam-se conversões explícitas (cast), como em C:
</p>

<p>(int) vari; // Converte a variável "vari" para o tipo inteiro</p>

<h4>Erros de Armazenamento</h4>

<ul>
  <li>
    <strong>Transbordamento (Overflow):</strong> Ocorre quando o resultado da operação
    é grande demais para a capacidade da variável de destino.
  </li>
  <li>
    <strong>Transbordamento Negativo (Underflow):</strong> Ocorre quando o resultado
    é tão pequeno que a variável não consegue representá-lo.
  </li>
</ul>

<h4>Sentenças de Atribuição</h4>

<p>
  As sentenças de atribuição definem o destino dos valores resultantes de
  operações na memória.
</p>

<ul>
  <li>A maioria das linguagens utiliza o sinal = (ex: C++, Java, Python).</li>
  <li>Exceções como Algol 60 e Ada utilizam :=.</li>
</ul>

<p>
  A estrutura padrão posiciona a variável que recebe o valor à esquerda e a
  expressão à direita:
</p>

<code>
  <pre>
  delta = b*b-4*a*c;
  </pre>
</code>

<h4>Atribuição de Listas (Múltiplas fontes e alvos)</h4>

<p>
  Algumas linguagens permitem atribuir vários valores a várias variáveis
  simultaneamente. Exemplo em Perl:
</p>

<code>
  <pre>
  ($primeiro, $segundo, $terceiro) = (10, 20, 30);
  </pre>
</code>

<h4>Operadores de Atribuição Compostos</h4>

<p>
  Funcionam como atalhos para modificar o valor de uma variável baseando-se nela
  mesma. Exemplo em linguagens baseadas em C:
</p>

<code>
  <pre>
  a += b; // Equivale a: a = a + b
</pre>
</code>

<p>
  <strong>Nota:</strong> O valor inicial da variável à esquerda é substituído e perdido
  após a execução.
</p>

<h4>Operadores de Atribuição Unários</h4>

<p>
  Atuam sobre uma única variável e alteram seu valor diretamente através de
  incremento ou decremento. Exemplos em linguagens baseadas em C:
</p>

<ul>
  <li>
    a = ++b; &rarr; A variável b é incrementada primeiro, e o novo valor é
    atribuído a a.
  </li>
  <li>
    a = b++; &rarr; O valor atual de b é atribuído a a, e depois b é
    incrementada.
  </li>
  <li>a++; &rarr; A variável a é simplesmente incrementada em uma unidade.</li>
</ul>

<h4>Atribuição como uma Expressão</h4>

<p>
  Muitas linguagens permitem realizar atribuições dentro de uma expressão maior.
  Exemplos:
</p>

<code>
  <pre>
  a = b + (c = d/b) - 1; // O resultado de d/b é salvo em c e usado no cálculo
  de a.
  a = b = 0; // Ambas as variáveis (a e b) recebem o valor zero.
  </pre>
</code>

<h3>Operadores Relacionais</h3>

<p>
  Os operadores relacionais servem para comparar os valores de dois operandos.
  Eles possuem uma precedência de execução baixa, o que significa que são
  avaliados após os operadores aritméticos. As sintaxes mais comuns nas
  linguagens de programação são:
</p>

<ul>
  <li><strong>Maior que:</strong> &gt;</li>
  <li><strong>Menor que:</strong> &lt;</li>
  <li><strong>Maior ou igual a:</strong> &gt;=</li>
  <li><strong>Menor ou igual a:</strong> &lt;=</li>
</ul>

<h4>Distinção entre Igualdade e Atribuição</h4>

<ul>
  <li>
    <strong>Igualdade (==):</strong> É o operador relacional utilizado para comparar
    se dois valores são iguais.
  </li>
  <li>
    <strong>Atribuição (=):</strong> É utilizado exclusivamente para definir o valor
    de uma variável. O uso invertido desses símbolos é um erro comum.
  </li>
</ul>

<h4>Variações do Operador "Diferente"</h4>

<p>
  A sintaxe para verificar se dois valores são diferentes varia conforme a
  linguagem:
</p>

<ul>
  <li><strong>Linguagens baseadas em C:</strong> !=</li>
  <li><strong>Ada:</strong> /=</li>
  <li><strong>Lua:</strong> ~=</li>
  <li><strong>Fortran 95:</strong> .NE. ou &lt;&gt;</li>
</ul>

<h3>Expressões Booleanas</h3>

<p>
  As expressões booleanas são construídas com base em variáveis, constantes,
  operadores lógicos e expressões relacionais. Elas operam com base em números
  binários e resultam exclusivamente em um de dois valores:
</p>

<ul>
  <li><strong>Verdadeiro:</strong> Geralmente representado por true ou 1.</li>
  <li><strong>Falso:</strong> Geralmente representado por false ou 0.</li>
</ul>

<h4>Exemplos de Expressões (em C++)</h4>

<ul>
  <li>
    <strong>(a &gt; b):</strong> Retorna verdadeiro se a for maior que b; caso contrário,
    retorna falso.
  </li>
  <li>
    <strong>(3 &lt= 2):</strong> Retorna invariavelmente falso, pois 3 não é menor
    ou igual a 2.
  </li>
  <li>
    <strong>(var1 == var2):</strong> Retorna verdadeiro se as variáveis forem exatamente
    iguais.
  </li>
  <li><strong>(3 == 3):</strong> Retorna verdadeiro.</li>
  <li><strong>(3 != 3):</strong> Retorna falso, pois 3 é igual a 3.</li>
</ul>

<h3>Álgebra Booleana</h3>

<p>
  A álgebra booleana opera com variáveis que possuem apenas dois estados
  possíveis: <strong>Verdadeiro (1)</strong> ou <strong>Falso (0)</strong>. Suas
  operações fundamentais substituem a aritmética tradicional e baseiam-se na
  lógica matemática. As ferramentas utilizadas para mapear todos os resultados
  possíveis dessas operações são chamadas de <strong>Tabelas Verdade</strong>.
</p>

<h4>Operações Lógicas Fundamentais</h4>

<ul>
  <li>
    <strong>NÃO (Inversão / Not):</strong> É uma operação unária que simplesmente
    inverte o estado atual da variável. Se a entrada for 0, o resultado é 1, e vice-versa.
  </li>
  <li>
    <strong>E (And):</strong> Requer dois operandos. O resultado só será
    <strong>verdadeiro</strong>
    se ambos os operandos forem simultaneamente verdadeiros. É utilizado para unir
    condições obrigatórias.
  </li>
  <li>
    <strong>OU (Or):</strong> Requer dois operandos. O resultado será
    <strong>verdadeiro</strong>
    se pelo menos um dos operandos for verdadeiro.
  </li>
  <li>
    <strong>OU EXCLUSIVO (Xor):</strong> O resultado será verdadeiro apenas quando
    os dois operandos tiverem valores diferentes entre si (um verdadeiro e um falso).
  </li>
</ul>

<h3>Precedência de Operadores</h3>

<p>
  Quando expressões misturam cálculos aritméticos, relacionais e lógicos, a
  execução segue uma ordem de prioridade estrita. Os parênteses () continuam
  sendo o recurso soberano para forçar ou modificar essa sequência. Em
  linguagens baseadas em C, a ordem de prioridade (da maior para a menor) é:
</p>

<ol>
  <li><strong>Incrementos pós-fixados:</strong> ++, --</li>
  <li>
    <strong>Operações unárias e negação:</strong> ++ / -- (pré-fixados), + / - (unários),
    ! (NÃO)
  </li>
  <li><strong>Multiplicação, divisão e resto:</strong> *, /, %</li>
  <li><strong>Adição e subtração binárias:</strong> +, -</li>
  <li><strong>Comparações de magnitude:</strong> &lt;, &gt;, &lt;=, &gt;=</li>
  <li><strong>Igualdade e diferença:</strong> ==, !=</li>
  <li><strong>Conjunção lógica (E):</strong> &&</li>
  <li><strong>Disjunção lógica (OU):</strong> ||</li>
</ol>

<h3>Exemplos Práticos de Expressões Combinadas</h3>

<ul>
  <li>
    <strong>(10 &lt; 20 && 30 &gt; 20):</strong> Resulta em
    <strong>verdadeiro</strong>, pois ambas as condições são verdadeiras.
  </li>
  <li>
    <strong>(10 &lt; 20 && 50 &gt; 50):</strong> Resulta em
    <strong>falso</strong>, porque a segunda condição é falsa (50 é igual a 50,
    não maior).
  </li>
  <li>
    <strong>(30 &gt;= 30 || 10 == 20):</strong> Resulta em
    <strong>verdadeiro</strong>, pois na operação OU basta que a primeira
    condição seja verdadeira.
  </li>
  <li>
    <strong>(10 != 10 || 20 &gt;= 21):</strong> Resulta em
    <strong>falso</strong>, já que ambas as condições testadas são falsas.
  </li>
  <li>
    <strong>(50 &gt; 20 && 40 &gt;= 10 || 10 &gt; 90):</strong> Resulta em
    <strong>verdadeiro</strong>. Pela regra de precedência, a operação && é
    avaliada primeiro entre as duas primeiras sentenças (gerando verdadeiro), e
    o resultado valida a operação || seguinte, mesmo com a última sentença sendo
    falsa.
  </li>
</ul>

<h3>Conclusão: Conceitos-Chave</h3>

<p>
  Esta etapa sintetiza os pontos fundamentais para a compreensão e a
  consolidação do conteúdo apresentado:
</p>

<ul>
  <li>
    <strong>Operadores e Operandos:</strong> As operações são realizadas sobre um,
    dois ou mais operandos através de operadores que variam conforme a linguagem
    de programação.
  </li>
  <li>
    <strong>Precedência e Organização:</strong> A ordem de execução aproveita regras
    da matemática, mas possui especificidades da computação. O uso de parênteses
    é o recurso utilizado para organizar e determinar a prioridade das ações.
  </li>
  <li>
    <strong>Conversão e Erros de Armazenamento:</strong> Modificar o tipo de uma
    variável pode alterar o seu valor original. Erros de cálculo podem ocorrer por
    overflow (limite máximo excedido) ou underflow (limite mínimo não alcançado).
  </li>
  <li>
    <strong>Atribuição:</strong> O símbolo de igual = é predominantemente utilizado
    para atribuir um valor a uma variável.
  </li>
  <li>
    <strong>Expressões Relacionais e Booleanas:</strong> Operadores como maior, menor
    ou igual comparam dois valores e geram uma resposta booleana (verdadeiro ou falso).
    Essas expressões tornam-se mais sofisticadas quando associadas pelos operadores
    lógicos NÃO, E e OU.
  </li>
</ul>
