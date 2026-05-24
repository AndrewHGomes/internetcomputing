<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Estruturas de Controle: Mecanismos de Tomada de Decisão</h2>

<Audios modulo="M3" aulas={["13", "14", "15", "16"]} />

<p>
  As estruturas de controle definem como o computador executa procedimentos a
  partir de condições iniciais. Elas permitem ao programador abstrair decisões
  reais e transformá-las em código, controlando o fluxo de execução do programa.
  A flexibilidade e o poder da programação baseiam-se em dois mecanismos
  principais:
</p>

<ul>
  <li>
    <strong>Seleção:</strong> Escolha entre caminhos distintos no fluxo de execução
    de sentenças.
  </li>
  <li>
    <strong>Iteração:</strong> Criação de uma repetição controlada de sentenças.
  </li>
</ul>

<h3>Desvio Incondicional</h3>

<p>
  O desvio incondicional é um mecanismo oriundo da programação de baixo nível
  que redireciona a execução do programa para uma posição específica e rotulada.
</p>

<ul>
  <li>
    <strong>Funcionamento:</strong> O programa "pula" diretamente para o ponto identificado.
  </li>
  <li><strong>Sintaxe comum:</strong> goto localDoPrograma</li>
  <li>
    <strong>Presença nas linguagens:</strong> Está incluído na maioria das linguagens,
    mas possui exceções como Java, Python e Ruby.
  </li>
  <li>
    <strong>Impacto:</strong> Apesar de simples e flexível, o seu uso diminui a confiabilidade
    dos programas.
  </li>
</ul>

<h3>Sentenças de Seleção</h3>

<p>
  As sentenças de seleção controlam o fluxo do programa permitindo o acesso a
  blocos distintos de código com base em uma expressão de controle
  pré-estabelecida. Elas são formadas por uma sentença de controle associada às
  sentenças que são controladas por ela.
</p>

<h4>Sentenças de Seleção de Dois Caminhos</h4>

<p>
  Essa estrutura avalia uma expressão de controle (uma "pergunta"). Se o
  resultado for verdadeiro, executa-se a "cláusula então"; se for falso,
  executa-se a "cláusula senão" (representada pela palavra-chave else).
</p>

<code>
  <pre>
    if expressão_de_Controle
      cláusula então
      cláusula senão
  </pre>
</code>

<h4>Variações de Sintaxe:</h4>

<ul>
  <li>
    <strong>Ruby e Lua:</strong> Utilizam `then` para iniciar o bloco e `end` para
    finalizá-lo
  </li>
  <li>
    <strong>Linguagens baseadas em C (e C++):</strong> A expressão de controle fica
    entre parênteses `( )` e os blocos são delimitados por chaves `&lbrace;&rbrace;`.
    As chaves são opcionais se a cláusula contiver apenas uma sentença.
  </li>
  <li>
    <strong>Fortran 95, Ada, Python e Ruby:</strong> Terminam a sequência da sentença
    com delimitadores como `end if`, `End If` ou apenas `end`.
  </li>
</ul>

<h4>Características Importantes:</h4>

<ul>
  <li>
    <strong>Aninhamento:</strong> É possível inserir seletores dentro de outros seletores,
    exigindo cuidado para evitar ambiguidades.
  </li>
  <li>
    <strong>Cláusula Senão (`else`):</strong> Não precisa de uma expressão de controle
    própria, pois é executada automaticamente se a condição do `if` for falsa.
  </li>
  <li>
    <strong>Opcionalidade:</strong> Se a cláusula senão não for necessária, o `else`
    pode ser descartado. Caso a expressão de controle seja falsa, o bloco do `if`
    simplesmente não é executado.
  </li>
</ul>

<h4>Sentenças de Seleção Múltipla</h4>

<p>
  A estrutura switch é utilizada para selecionar uma entre várias sentenças ou
  grupos de sentenças. Embora sua função possa ser substituída por uma série de
  estruturas if, o switch facilita a legibilidade do programa.
</p>

<code>
  <pre>
    switch (expressão)
    &lbrace;
      case opção1:
      sentenças1;
      break;
      case opção2:
      sentenças2;
      break;
      default:
      sentença padrão;
    &rbrace;
  </pre>
</code>

<h4>Funcionamento da Estrutura</h4>

<ul>
  <li>
    <strong>Análise inicial:</strong> A variável presente na expressão é avaliada
    na primeira sentença.
  </li>
  <li>
    <strong>Redirecionamento:</strong> A execução é desviada para o case correspondente
    ao valor da expressão.
  </li>
  <li>
    <strong>Execução e interrupção:</strong> As sentenças internas do case são executadas
    até que o comando break seja encontrado, o qual encerra a execução do switch.
  </li>
  <li>
    <strong>Caso padrão (default):</strong> Se a variável não corresponder a nenhum
    dos valores dos cases, o programa salta para o identificador default, executa
    a sentença padrão e encerra o bloco.
  </li>
</ul>

<h3>Exemplos de Estruturas de Seleção</h3>

<h4>Seleção Simples com if</h4>

<p>
  O exemplo abaixo compara duas variáveis e altera o valor de uma terceira caso
  a condição seja verdadeira. Os comentários explicam o funcionamento:
</p>

<code>
  <pre>
  int a = 1; // declaração de variável
  int b = 2; // declaração de variável
  float c = 9.1; // declaração de variável

  if (a &lt; b) // uso do if: compara se a é menor que b
  &lbrace;
    c = 10.1; // sentença executada se a &lt; b. Caso contrário, c permanece com
    9.1
  &lbrace;
  </pre>
</code>

<h4>Saída de Dados (cout)</h4>

<p>A sintaxe geral para exibição de dados no monitor em C++ é:</p>

<code>
  <pre>cout &lt;&lt; "texto" &lt;&lt; variavel &lt;&lt; "texto";</pre>
</code>

<p>
  Não há limitações quanto ao ordenamento de variáveis e textos no comando cout.
</p>

<h4>Seleção Composta com if e else</h4>

<p>Este exemplo implementa um seletor para evitar a divisão por zero:</p>

<code>
  <pre>
  int a, b; 
  a = 10; 
  b = 5; 

  if (b != 0) 
  &lbrace;
    float c = a / b;
    cout &lt;&lt; "o resultado eh " &lt;&lt; c &lt;&lt; "\n";
  &rbrace; 
  else 
  &lbrace;
    cout &lt;&lt; "divisao por zero\n"; 
  &rbrace;
  </pre>
</code>

<ul>
  <li><strong>Saída no monitor para este caso:</strong> o resultado eh 2</li>
  <li>
    <strong>Explicação:</strong> Como o valor de b não é zero, o primeiro bloco é
    executado. Se b fosse zero, a saída seria divisao por zero.
  </li>
</ul>

<h4>Seleção Dupla com if Aninhados</h4>

<p>Exemplo que verifica se as variáveis a e b são nulas:</p>

<code>
  <pre>
  int a, b; 
  a = 10; 
  b = 0; 

  if (b == 0) 
  &lbrace; 
    cout &lt;&lt; "b eh nulo\n"; 
    if (a == 0) 
    &lbrace; 
        cout &lt;&lt; "a tambem eh nulo\n"; 
    &rbrace; 
  &rbrace;
  </pre>
</code>

<ul>
  <li><strong>Saída no monitor para este caso:</strong> b eh nulo</li>
  <li>
    <strong>Cenários alternativos:</strong>
    <ul>
      <li>
        Se a e b fossem zero, seriam exibidas as duas frases (b eh nulo e a
        tambem eh nulo).
      </li>
      <li>Se ambos fossem diferentes de zero, a tela ficaria vazia.</li>
    </ul>
  </li>
</ul>

<h4>Entrada de Dados (cin) e Seleção Múltipla (switch)</h4>

<p>
  A instrução para entrada de dados via teclado adota a sintaxe cin &gt;&gt;
  variável;. O exemplo abaixo utiliza essa instrução junto com a estrutura
  switch:
</p>

<code>
  <pre>
  cin &gt;&gt; x; // instrução de entrada de dados realizada pelo teclado

  switch(x) 
  &lbrace; 
      case 1: 
          cout &lt;&lt; "selecionou o numero um\n"; 
          break; 
      case 2: 
          cout &lt;&lt; "selecionou o numero dois\n"; 
          break; 
      case 3: 
          cout &lt;&lt; "selecionou o numero tres\n"; 
          break; 
      default: 
          cout &lt;&lt; "selecao desconhecida\n"; 
  &rbrace;
  </pre>
</code>

<ul>
  <li>
    <strong>Saída no monitor:</strong> O texto exibido depende exclusivamente do
    dado inserido pelo usuário.
  </li>
</ul>

<h3>Sentenças de Iteração</h3>

<p>
  A sentença de iteração faz com que uma ou mais sentenças sejam executadas
  zero, uma ou mais vezes. Sua principal função é repetir laços (trechos de
  código) de forma definida ou indefinida. O corpo do laço é o conjunto de
  sentenças controlado pela iteração. A construção pode ocorrer de duas formas:
</p>

<ul>
  <li>
    <strong>Pré-teste:</strong> A validação ocorre antes da execução do corpo.
  </li>
  <li>
    <strong>Pós-teste:</strong> A validação ocorre depois da execução do corpo.
  </li>
</ul>

<h4>Laços Controlados por Contador (for)</h4>

<p>
  Geralmente implementado com a instrução for, esse laço baseia-se em uma
  contagem e inclui: variável de laço (contador), valores inicial e final (ou
  condição de contagem) e o passo da contagem (diferença entre os valores).
</p>

<h4>Funcionamento do for</h4>

<p>
  A contagem começa na inicialização da variável. O controle testa a condição:
  se for verdadeira, o corpo do laço é executado e o incremento ou decremento é
  realizado. O valor do contador muda e a condição é testada novamente. O laço
  encerra quando o valor da variável não é mais aceito pelo controle.
</p>

<ul>
  <li>
    <strong>Python:</strong>
    <pre>
  for variavel_do_laco in objeto:
    corpo do laço
    </pre>
  </li>
  <li>
    <strong>Linguagens baseadas em C (incluindo C++):</strong>
    <pre>
  for (inicialização; controle; incremento)
  &lbrace;
    corpo do laço
  &rbrace;
    </pre>
  </li>
</ul>

<h4>Laços Controlados Logicamente</h4>

<p>
  Esses laços executam um escopo repetidamente enquanto uma expressão booleana
  for verdadeira. São divididos em dois tipos principais:
</p>

<h4>Pré-teste (while)</h4>

<p>
  Realiza a validação condicional antes da primeira execução. Se o resultado
  inicial for falso, o corpo do laço não é executado nenhuma vez. O programa
  repete o bloco enquanto a condição for verdadeira e sai do laço assim que ela
  se tornar falsa.
</p>

<ul>
  <li>
    <strong>Sintaxe em linguagens baseadas em C:</strong>
    <pre>
    while (controle)
    &lbrace;
      corpo do laço
    &rbrace;
    </pre>
  </li>
</ul>

<h4>Pós-teste (do-while)</h4>

<p>
  Realiza o teste de controle apenas após a execução do bloco. Isso garante que
  o corpo do laço seja executado ao menos uma vez, sem testes prévios. Após a
  primeira passagem, a condição é testada e o laço se repete até que a expressão
  seja falseada.
</p>

<ul>
  <li>
    <strong>Sintaxe em linguagens baseadas em C:</strong>
    <pre>
    do &lbrace;
      corpo do laço
    &rbrace; while (controle);
    </pre>
  </li>
</ul>

<h4>Saídas Rotuladas</h4>

<p>
  Artifício utilizado para interromper a execução de um laço antes do seu fim
  determinado. O comando encerra o laço "no meio" da execução:
</p>

<ul>
  <li><strong>break:</strong> Utilizado em C, C++, C#, Python, Ruby e Java.</li>
  <li><strong>last:</strong> Utilizado em Perl.</li>
</ul>

<h3>Exemplos de Estruturas de Iteração</h3>

<h4>Repetição com for</h4>

<p>
  Este exemplo exibe na tela os números inteiros de 1 a 100. A sequência \t
  inserida no cout equivale ao espaçamento de um "tab" no teclado.
</p>

<code>
  <pre>
  // mostrar os inteiros de 1 a 100 
  for (int x = 1 ; x &lt;= 100 ; x = x + 1) 
  &lbrace; 
      cout &lt;&lt; x &lt;&lt; "\t"; 
  &rbrace;
  </pre>
</code>

<ul>
  <li>
    <strong>Saída no monitor:</strong> Os números de 1 a 100 separados por espaçamento
    horizontal (1 2 3 ... 100).
  </li>
</ul>

<h4>Repetição com for Aninhado</h4>

<p>
  É possível realizar repetições dentro de repetições. O exemplo abaixo aninha
  dois laços for para exibir cada número em uma nova linha com a quantidade de
  repetições correspondente ao seu próprio valor.
</p>

<code>
  <pre>
  /* mostrar na tela 1x o num 1, 2x o num 2, ...*/ 
  for (int linha = 1 ; linha &lt;= 9 ; linha++) 
  &lbrace;
    for (int coluna = 1 ; coluna &lt;= linha ; coluna++) 
    &lbrace; 
        cout &lt;&lt; linha; // mostra na tela somente um único dígito por iteração
    &rbrace; 
    cout &lt;&lt; "\n"; 
  &rbrace;
  </pre>
</code>

<ul>
  <li>
    <strong>Saída no monitor:</strong>
    <pre>
    1
    22
    333
    4444
    55555
    666666
    7777777
    88888888
    999999999
    </pre>
  </li>
</ul>

<h4>Repetição com while (Pré-teste)</h4>

<p>
  O bloco abaixo valida a condição antes da execução e exibe mensagens
  consecutivas até que o usuário insira o caractere esperado.
</p>

<code>
  <pre>
  // espera o usuario digitar a letra "a" 
  char ch; 
  cin &gt;&gt; ch;

  while(ch != 'a') 
  &lbrace;
    cout &lt;&lt; "letra incorreta\n"; 
    cin &gt;&gt; ch; 
  &rbrace;
  cout &lt;&lt; "letra correta\n";
  </pre>
</code>

<ul>
  <li>
    <strong>Funcionamento:</strong> O programa exibe repetidamente o texto letra
    incorreta enquanto o valor de ch for diferente de 'a'. Assim que 'a' é digitado,
    o laço encerra e exibe letra correta.
  </li>
</ul>

<h4>Repetição com do-while (Pós-teste)</h4>

<p>
  Este exemplo executa o bloco de instruções obrigatoriamente a primeira vez e
  mantém a repetição para acumular a soma dos números fornecidos pelo usuário.
</p>

<code>
  <pre>
  // mostra a soma de todos os numeros digitados 
  // fecha a operação quando a entrada for 0 
  float numero, soma; 

  do &lbrace; 
    cout &lt;&lt; "digite um número\n"; 
    cin &gt;&gt; numero; 
    soma += numero; 
  &rbrace; while(numero != 0); 

  cout &lt;&lt; "a soma dos valores eh " &lt;&lt; soma;
  </pre>
</code>

<ul>
  <li>
    <strong>Funcionamento:</strong> O texto digite um número aparece em laço na tela
    e os valores são somados. A repetição é interrompida apenas quando o valor digitado
    na entrada for zero, exibindo o resultado final da soma.
  </li>
</ul>

<h3>Conclusão: Conceitos-chave</h3>

<p>
  As <strong>sentenças de controle</strong> são responsáveis por tomar decisões dentro
  de um programa. Elas são subdivididas de acordo com a sua aplicação de seleção
  ou de iteração:
</p>

<h4>Sentenças de Seleção (Tomada de Decisão)</h4>

<ul>
  <li>
    <strong>if:</strong> Utilizado para selecionar entre executar ou não um bloco
    de código com base em uma condição.
  </li>
  <li>
    <strong>if-else:</strong> Utilizado para selecionar entre dois blocos distintos
    com base em uma condição.
  </li>
  <li>
    <strong>switch (ou if elaborados):</strong> Utilizado para selecionar entre vários
    caminhos possíveis com base em opções predefinidas.
  </li>
</ul>

<h4>Sentenças de Iteração (Repetição)</h4>

<ul>
  <li>
    <strong>for:</strong> Utilizado para repetir um bloco de código por um número
    determinado de vezes.
  </li>
  <li>
    <strong>while:</strong> Utilizado para repetir um bloco de código dependendo
    de uma condição (com validação prévia).
  </li>
  <li>
    <strong>do-while:</strong> Utilizado para repetir um bloco dependendo de uma
    condição, mas garantindo que o bloco seja executado ao menos uma vez antes do
    teste.
  </li>
</ul>
