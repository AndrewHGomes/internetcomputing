<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Subprogramas</h2>

<Audios modulo="M3" aulas={["17", "18", "19", "20"]} />

<h3>O que é um Subprograma</h3>

<p>
  Um subprograma é um bloco de sentenças executado a partir de uma
  sentença-chave no programa principal. Sua principal função é evitar a
  reescrita de códigos para rotinas que se repetem, o que abstrai detalhes e
  aumenta a legibilidade do sistema.
</p>

<h4>Categorias de Subprogramas</h4>

<ul>
  <li>
    <strong>Procedimento:</strong> Executa uma computação a partir de parâmetros
    recebidos.
  </li>
  <li>
    <strong>Função:</strong> Funciona como uma função matemática, recebendo um ou
    mais valores e devolvendo um novo valor.
  </li>
</ul>

<h4>Características Principais</h4>

<ul>
  <li>Possui apenas um ponto de entrada.</li>
  <li>O programa principal é suspenso durante a execução do subprograma.</li>
  <li>
    O controle da execução retorna ao programa principal assim que o subprograma
    termina.
  </li>
  <li>
    <strong>Exceção:</strong> As corrotinas quebram essa regra, pois rodam paralelamente
    entre si.
  </li>
</ul>

<h3>Estrutura Básica de um Subprograma</h3>

<p>
  Um subprograma funciona como um "departamento" separado do programa principal,
  situado fora de seu escopo. Ele entra em estado ativo assim que é chamado e
  permanece nessa condição até concluir sua execução. A implementação divide-se
  em duas partes:
</p>

<ul>
  <li>
    <strong>Definição:</strong> Escrita externa ao programa principal que descreve
    as entradas, saídas e ações do subprograma.
  </li>
  <li>
    <strong>Chamada:</strong> Pedido explícito de execução feito dentro do programa
    principal, incluindo os parâmetros necessários.
  </li>
</ul>

<h4>Componentes da Definição</h4>

<p>Um subprograma é constituído por um cabeçalho e por um escopo:</p>

<ul>
  <li>
    <strong>Cabeçalho:</strong> Contém o nome do subprograma e os parâmetros
    necessários para sua ativação.
    <ul>
      <li><strong>Em C++:</strong> void nome_do_subprograma (parâmetros)</li>
      <li>
        <strong>Em Ada:</strong> procedure nome_do_subprograma (parâmetros)
      </li>
      <li><strong>Em Python:</strong> def nome_do_subprograma (parâmetros)</li>
    </ul>
  </li>
  <li>
    <strong>Escopo:</strong> Conjunto de sentenças executadas a cada chamada. Cada
    linguagem possui sua forma de agrupamento (no C++, por exemplo, utilizam-se chaves
    &lbrace;&rbrace;).
  </li>
</ul>

<h4>Funcionamento e Parâmetros</h4>

<p>O fluxo de execução segue etapas específicas baseadas na troca de dados:</p>

<ol>
  <li>
    <strong>Interrupção:</strong> O programa principal interrompe sua execução
    na linha da chamada e envia os <strong>parâmetros reais</strong> (valores atuais)
    para o subprograma.
  </li>
  <li>
    <strong>Associação:</strong> O subprograma recebe esses dados por meio de
    seus
    <strong>parâmetros formais</strong> (variáveis declaradas no cabeçalho). A associação
    ocorre estritamente pela ordem de apresentação (1º parâmetro real no 1º parâmetro
    formal, e assim por diante).
  </li>
  <li>
    <strong>Retorno:</strong> Após processar as sentenças, o controle volta ao programa
    principal, podendo entregar um ou nenhum valor de retorno.
  </li>
  <li>
    <strong>Importante:</strong> Os subprogramas possuem
    <strong>variáveis locais</strong>, que são declaradas dentro do seu escopo e
    funcionam exclusivamente dentro dele.
  </li>
</ol>

<h3>Exemplos de Subprogramas</h3>

<h4>Função</h4>

<p>
  A função é um tipo de subprograma que calcula e retorna um valor para o
  programa principal.
</p>

<h4>Exemplo de Chamada no Programa Principal:</h4>

<code>
  <pre>
    m1 = media (v1, v2, v3);
  </pre>
</code>

<p>
  (Considerando as variáveis m1, v1, v2, v3 previamente declaradas como float).
</p>

<h4>Funcionamento Passo a Passo:</h4>

<ul>
  <li>
    <strong>Cabeçalho:</strong> Declarado como float media (float a, float b, float
    c). O termo float inicial define o tipo do dado que retornará ao programa principal.
    Os parâmetros formais (a, b, c) recebem e armazenam, respectivamente, os valores
    dos parâmetros reais (v1, v2, v3).
  </li>
  <li>
    <strong>Escopo:</strong> Delimitado por chaves &lbrace; &rbrace;, contém as ações
    do subprograma.
  </li>
  <li>
    <strong>Processamento:</strong> Realiza o cálculo da média simples: x = (a +
    b + c) / 3;.
  </li>
  <li>
    <strong>Retorno:</strong> A última sentença é return x;. Ela encerra o subprograma
    e envia o valor contido na variável local x de volta para o programa principal,
    que o armazena em m1.
  </li>
  <li>
    <strong>Isolamento de Escopo:</strong> O subprograma não tem acesso às variáveis
    do programa principal (m1, v1, v2, v3), e o programa principal não acessa as
    variáveis da função (x, a, b, c). A comunicação ocorre exclusivamente através
    da chamada e do retorno.
  </li>
</ul>

<h4>Procedimento</h4>

<p>
  O procedimento é um tipo de subprograma que executa uma ação, mas não retorna
  valores para o programa principal.
</p>

<h4>Exemplo de Chamada no Programa Principal:</h4>

<code>
  <pre>
    faixa ();
  </pre>
</code>

<p>
  (Não necessita ser atribuído a nenhuma variável, pois não gera valor de
  retorno).
</p>

<h4>Funcionamento Passo a Passo:</h4>

<ul>
  <li>
    <strong>Cabeçalho:</strong> Declarado como void faixa (). O termo void (vazio)
    indica que o subprograma não retorna variáveis. Os parênteses vazios indicam
    que ele também não precisa receber parâmetros.
  </li>
  <li><strong>Escopo:</strong> Delimitado por chaves &lbrace; &rbrace;.</li>
  <li>
    <strong>Processamento:</strong> Contém apenas a ação direta de imprimir uma sequência
    de caracteres de cerquilha (#). Não apresenta a sentença return.
  </li>
</ul>

<h3>O Programa "Olá, Mundo!"</h3>

<p>
  O programa "Olá, Mundo!" (ou Hello, World) é tradicionalmente a primeira
  implementação feita ao se aprender uma nova linguagem de programação. Ele
  serve como um "marco zero" para entender a sintaxe básica e garantir que o
  ambiente de desenvolvimento esteja funcionando corretamente.
</p>

<h4>Implementação em Diferentes Linguagens</h4>

<ul>
  <li>
    <strong>Ada:</strong>
    <pre>
      with Ada.Text_IO; use Ada.Text_IO;
      procedure Ola is
      begin
        Put_Line ("Ola, mundo!");
      end Ola;
    </pre>
  </li>
  <li>
    <strong>C:</strong>
    <pre>
      #include &lt;stdio.h&gt;
      int main() &lbrace;
        printf("Ola, mundo!\n")
      &rbrace;
    </pre>
  </li>
  <li>
    <strong>C++:</strong>
    <pre>
      #include &lt;iostream&gt; 
      using namespace std;   
      int main() &lbrace;
        cout &lt;&lt; "Ola, mundo!\n"; 
      &rbrace;
    </pre>
  </li>
  <li>
    <strong>C#</strong>
    <pre>Console.WriteLine("Ola, mundo!");</pre>
  </li>
  <li>
    <strong>Fortran:</strong>
    <pre>
      program Ola 
        print *, "Ola, mundo!" 
      end program Ola
    </pre>
  </li>
  <li>
    <strong>Java:</strong>
    <pre>
      public class Main &lbrace;
        public static void main(String[] args) &lbrace;
          System.out.println("Ola, mundo!"); 
        &rbrace;
      &rbrace;
    </pre>
  </li>
  <li>
    <strong>Lisp:</strong>
    <p>(print "Ola, mundo!")</p>
  </li>
  <li>
    <strong>Lua:</strong>
    <pre>print("Ola, mundo!")</pre>
  </li>
  <li>
    <strong>Pascal (Delphi):</strong>
    <pre>
      program Alo; 
      begin 
        writeln ('Ola, mundo!'); 
      end.
    </pre>
  </li>
  <li>
    <strong>Perl:</strong>
    <pre>print "Ola, mundo!\n";</pre>
  </li>
  <li>
    <strong>Python:</strong>
    <pre>print("Ola, mundo!")</pre>
  </li>
  <li>
    <strong>Ruby:</strong>
    <pre>puts "Ola, mundo!"</pre>
  </li>
</ul>

<h4>Ferramentas para Testes (Compiladores Online)</h4>

<p>
  Para testar e rodar esses códigos sem a necessidade de instalar múltiplos
  ambientes de desenvolvimento no computador, recomenda-se o uso de compiladores
  e depuradores online. Eles são ideais para programas simples e exemplos de
  estudo. Algumas plataformas disponíveis:
</p>

<ul>
  <li><strong>Online GDB</strong> (onlinegdb.com)</li>
  <li><strong>Programiz</strong> (programiz.com)</li>
  <li><strong>Replit</strong> (replit.com)</li>
</ul>

<h3>Exemplos de Programas em C++</h3>

<h4>Exemplo 1: Estrutura Básica e Condicional if-else</h4>

<p>
  Este exemplo introduz a anatomia fundamental de um código em C++ e o desvio
  condicional.
</p>

<ul>
  <li>
    <strong>Preâmbulo Padrão:</strong> Composto pela inclusão da biblioteca de entrada
    e saída (#include &lt;iostream&gt;) e pela definição do espaço de nomes (using
    namespace std;). Deve ser repetido na abertura dos programas.
  </li>
  <li>
    <strong>Variáveis Globais:</strong> Declaradas logo após o preâmbulo (fora de
    funções), sendo válidas em todo o escopo do programa.
  </li>
  <li>
    <strong>Função Principal (main):</strong> Ponto de início obrigatório de todo
    programa C++. Seu escopo é delimitado por chaves &lbrace; &rbrace;.
  </li>
  <li>
    <strong>Indentação:</strong> Uso de espaçamento (tabulação) à direita para organizar
    os blocos de código e aumentar a legibilidade.
  </li>
  <li>
    <strong>Entrada e Saída de Dados:</strong> * cout: Exibe mensagens na tela.
    O caractere \n dentro das aspas indica uma quebra de linha.
    <ul>
      <li>cin: Recebe dados do usuário e os armazena nas variáveis.</li>
    </ul>
  </li>
  <li>
    <strong>Estrutura if-else:</strong> Avalia uma condição. Se a expressão dentro
    do if for verdadeira, executa o seu respectivo bloco de chaves; caso contrário
    (else), o programa desvia a execução para o bloco alternativo.
  </li>
</ul>

<h4>Exemplo 2: Estrutura de Seleção Múltipla switch</h4>

<p>
  Ideal para fluxos com múltiplas opções baseadas em uma única variável, como
  uma calculadora.
</p>

<ul>
  <li>
    <strong>Tipos de Dados:</strong> Utiliza char (caractere) para armazenar o símbolo
    da operação e float (ponto flutuante) para valores reais e resultados.
  </li>
  <li>
    <strong>O Condicional switch:</strong> Avalia a variável da operação e direciona
    o fluxo para o case correspondente.
  </li>
  <li>
    <strong>Sintaxe dos cases:</strong> Os caracteres de comparação são escritos
    entre aspas simples (ex: 'A'). Cada caso contém suas expressões aritméticas e
    comandos de saída.
  </li>
  <li>
    <strong>Sentença break:</strong> Encerra a execução do case. Ela faz o programa
    ignorar o restante do bloco switch e saltar diretamente para as linhas após o
    seu fechamento.
  </li>
  <li>
    <strong>Cláusula default:</strong> Atua como um caso padrão de segurança. Se
    o valor inserido não corresponder a nenhum dos cases definidos, o programa executa
    o bloco do default (ex: exibindo "operação inválida").
  </li>
</ul>

<h4>Exemplo 3: Estrutura de Repetição for e Comentários Longos</h4>

<p>
  Aborda laços de repetição numéricos e uma forma alternativa de documentação.
</p>

<ul>
  <li>
    <strong>Comentários de Múltiplas Linhas:</strong> Delimitados por /* no início
    e */ no fim, servindo como alternativa ao // para blocos grandes de texto.
  </li>
  <li>
    <strong>Laço for:</strong> Controla uma repetição baseando-se em três etapas
    na sua instrução inicial:
    <ol>
      <li>
        <strong>Inicialização:</strong> Define o ponto de partida da contagem (ex:
        x = 1;).
      </li>
      <li>
        <strong>Condição:</strong> Mantém o laço ativo enquanto a expressão for verdadeira
        (ex: x &lt; 100;).
      </li>
      <li>
        <strong>Incremento:</strong> Atualiza a variável a cada iteração usando o
        operador x++ (equivalente a x = x + 1).
      </li>
    </ol>
  </li>
</ul>

<h4>Exemplo 4: Manipulação de Matrizes (Vetores)</h4>

<p>
  Demonstra o armazenamento estruturado de dados e o uso de laços combinados.
</p>

<ul>
  <li>
    <strong>Matriz (Vetor):</strong> Estrutura de dados utilizada para agrupar e
    armazenar múltiplos valores de um mesmo tipo sob o mesmo nome (como as notas
    dos alunos).
  </li>
  <li>
    <strong>Acesso por Índice:</strong> Os dados são carregados e lidos indicando
    a posição do índice dentro de colchetes, começando em zero (ex: notas[0], notas[1],
    etc.).
  </li>
  <li>
    <strong>Laços Combinados:</strong> Utiliza duas estruturas for independentes
    no código:
    <ul>
      <li>
        O primeiro laço serve para capturar os dados via cin e preencher as
        posições da matriz.
      </li>
      <li>
        O segundo laço realiza a leitura sequencial dessas posições para
        acumular os valores na variável soma.
      </li>
    </ul>
  </li>
  <li>
    <strong>Flexibilidade do Código:</strong> O tamanho da matriz e o limite dos
    laços (fixados em 5) podem ser parametrizados substituindo o número fixo por
    uma variável definida pelo usuário, permitindo calcular a média de qualquer quantidade
    de alunos.
  </li>
</ul>

<h4>Exemplo 5: Implementação de Procedimento com Condicionais Lógicos</h4>

<p>
  Exemplifica a aplicação prática de subprogramas sem retorno em cenários de
  conversão e validação.
</p>

<ul>
  <li>
    <strong>Definição do Procedimento:</strong> Criado sob o identificador saudacao.
    O cabeçalho indica que ele aceita duas variáveis inteiras como parâmetros e usa
    o tipo void, explicitando que não devolve valores ao final.
  </li>
  <li>
    <strong>Processamento Interno:</strong> Transforma as entradas de horas e minutos
    em um formato decimal correspondente (ex: converte 13h30min para 13,5h) através
    de uma expressão algébrica.
  </li>
  <li>
    <strong>Operadores Lógicos no if:</strong> Para validar se o horário está contido
    em um intervalo específico, as condições combinam os operadores relacionais "maior
    ou igual" (&gt;=) e "menor" (&lt;) unidos pelo operador lógico "E" (&&).
  </li>
  <li>
    <strong>Sintaxe Simplificada:</strong> Quando um bloco if contém apenas uma sentença
    a ser executada, a utilização de chaves &lbrace; &rbrace; torna-se opcional.
  </li>
  <li>
    <strong>Chamada no Programa Principal:</strong> A execução é disparada diretamente
    pelo nome do subprograma passando os parâmetros requeridos, sem a necessidade
    de atribuir a chamada a nenhuma variável.
  </li>
</ul>

<h3>Conclusão: Conceitos-chave</h3>

<h4>Subprogramas</h4>

<p>
  São pequenos trechos de código isolados do programa principal, desenvolvidos
  para executar rotinas específicas que precisam ser repetidas diversas vezes ao
  longo do sistema. Sua separação evita a duplicidade de código e organiza o
  software de forma modular.
</p>

<h4>Classificação e Escopo</h4>

<ul>
  <li>
    <strong>Procedimentos:</strong> Subprogramas projetados para realizar ações de
    caráter geral.
  </li>
  <li>
    <strong>Funções:</strong> Subprogramas estruturados para receber dados, processá-los
    e responder obrigatoriamente com um valor de retorno.
  </li>
  <li>
    <strong>Variáveis Locais:</strong> Variáveis específicas declaradas dentro do
    escopo do subprograma para manipular os parâmetros e valores recebidos, operando
    de forma isolada do restante do programa.
  </li>
</ul>

<h4>O Ponto de Partida na Programação</h4>

<p>
  O programa "Olá, Mundo!" é o modelo ideal e mais simples para iniciar o
  aprendizado em qualquer linguagem de programação. Restringindo-se a apenas
  exibir essa mensagem na tela, ele funciona como a base prática para
  compreender a sintaxe de novos códigos e dar início ao domínio de uma nova
  linguagem.
</p>
