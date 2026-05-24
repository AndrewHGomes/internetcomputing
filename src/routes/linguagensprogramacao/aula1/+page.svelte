<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Aspectos Preliminares da Linguagem de Programação</h2>

<Audios modulo="M3" aulas={["01", "02", "03", "04"]} />

<h3>Introdução e Objetivos</h3>

<p>
  Os sistemas computacionais e os dispositivos programados estão presentes na
  maioria das atividades diárias modernas, o que torna o conhecimento das
  linguagens de programação e de sua lógica fundamental. O estudo desta etapa
  abrange:
</p>

<ul>
  <li>Aspectos preliminares e classificações.</li>
  <li>Categorias das linguagens de programação.</li>
  <li>Sintaxe, semântica, análise léxica e análise sintática.</li>
</ul>

<p>
  O objetivo principal é capacitar a escolha da melhor linguagem para cada
  aplicação, além de descrever e prever os resultados do código programado.
</p>

<h3>Aspectos Preliminares</h3>

<p>
  Não existe uma "melhor linguagem de programação". As linguagens possuem
  implementações distintas para atender a diferentes áreas e aplicações; uma
  linguagem eficiente para um cenário pode ser inadequada ou ineficiente para
  outro.
</p>

<h4>Exemplos de Aplicações e Linguagens</h4>

<p>
  As linguagens de programação são desenvolvidas para objetivos específicos,
  destacando-se em seus respectivos campos:
</p>

<ul>
  <li><strong>Aplicações Científicas:</strong> ALGOL, Fortran e MATLAB.</li>
  <li><strong>Aplicações Empresariais:</strong> COBOL.</li>
  <li><strong>Inteligência Artificial:</strong> LISP e Prolog.</li>
  <li><strong>Programação de Sistemas:</strong> Linguagens baseadas em C.</li>
  <li><strong>Softwares para Web:</strong> XHTML e Java.</li>
</ul>

<p>
  O foco principal do conteúdo será direcionado às linguagens baseadas em C,
  como C, C++, Java e C#.
</p>

<h3>Fatores para Escolha de uma Linguagem de Programação</h3>

<p>
  A escolha da melhor linguagem para um projeto depende de fatores técnicos e
  humanos, indo além da área de aplicação. A análise baseia-se em quatro
  critérios principais: legibilidade, capacidade de escrita, confiabilidade e
  custo.
</p>

<h4>Legibilidade</h4>

<p>
  É a facilidade de leitura e compreensão do código. Ela depende de cinco
  características:
</p>

<ul>
  <li>
    <strong>Simplicidade:</strong> Quantidade de construções básicas da linguagem.
    Muitas instruções e definições tornam o aprendizado mais difícil.
  </li>
  <li>
    <strong>Multiplicidade de recursos:</strong> Quantidade de maneiras diferentes
    de realizar a mesma operação. O excesso de opções eleva a dificuldade de compreensão.
  </li>
  <li>
    <strong>Sobrecarga de operadores:</strong> Um único operador possuir múltiplos
    significados. O excesso dificulta a leitura e gera erros, mas a simplicidade
    extrema (como no Assembly) também reduz a legibilidade.
  </li>
  <li>
    <strong>Ortogonalidade:</strong> O grau de redundância entre as sentenças, determinando
    o quanto uma instrução pode "invadir" a área de atuação de outra.
  </li>
  <li>
    <strong>Tipos de dados:</strong> Presença de mecanismos adequados para representar
    dados (ex: usar true para verdadeiro é mais legível do que usar o binário 1).
  </li>
  <li>
    <strong>Sintaxe:</strong> Uso eficiente de palavras especiais e forte vínculo
    entre forma e significado (ex: o uso de if para a condição "se").
  </li>
</ul>

<h4>Capacidade de Escrita</h4>

<p>
  É a facilidade de codificar na linguagem. Compartilha os conceitos de
  simplicidade e ortogonalidade, além de depender de:
</p>

<ul>
  <li>
    <strong>Abstração:</strong> Capacidade de usar estruturas sofisticadas que exigem
    menos atenção aos detalhes de baixo nível.
  </li>
  <li>
    <strong>Expressividade:</strong> Presença de operadores poderosos que permitem
    criar programas mais curtos.
  </li>
</ul>

<h4>Confiabilidade</h4>

<p>
  Mede se o programa executa estritamente de acordo com suas especificações. Uma
  linguagem é mais confiável quando possui:
</p>

<ul>
  <li>Mecanismos para verificação de erros de digitação.</li>
  <li>
    Tratamento de exceções (interceptação e correção de erros em tempo de
    execução).
  </li>
  <li>
    Uso correto de apelidos (múltiplos nomes acessando a mesma célula de
    memória).
  </li>
  <li>Boa legibilidade e capacidade de escrita.</li>
</ul>

<h4>Custo</h4>

<p>
  O impacto financeiro e de tempo no ciclo de vida do software. O custo envolve:
</p>

<ul>
  <li>Treinamento de programadores na linguagem.</li>
  <li>Tempo gasto na escrita do código.</li>
  <li>Processos de compilação e execução.</li>
  <li>Implementação do código e otimização da velocidade de execução.</li>
  <li>
    <strong>Manutenção:</strong> Correção de erros e modificações para novas funcionalidades
    em programas já desenvolvidos.
  </li>
</ul>

<h3>Categorias de Linguagens de Programação</h3>

<p>
  As linguagens de programação são divididas em quatro categorias principais:
</p>

<ul>
  <li>
    <strong>Imperativas:</strong> Os recursos centrais são variáveis, instruções
    de atribuição e iteração. Inclui linguagens que suportam orientação a objetos,
    linguagens de scripting e linguagens visuais. Exemplos: C, Java, Perl, JavaScript,
    Visual BASIC .NET e C++.
  </li>
  <li>
    <strong>Funcionais:</strong> O meio principal de realizar cálculos é a aplicação
    de funções a parâmetros determinados. Exemplos: LISP, Scheme, ML e F#.
  </li>
  <li>
    <strong>Lógicas:</strong> São baseadas em regras, sem especificação de ordem
    própria. Exemplo: Prolog.
  </li>
  <li>
    <strong>Marcas/Programação Híbridas:</strong> Linguagens de marcação estendidas
    para suportar programação. Exemplos: JSTL, XSLT e LaTeX (utilizado na escrita
    de livros e artigos científicos, focando no conteúdo e automatizando a formatação,
    diferentemente de editores WYSIWYG como o Microsoft Word).
  </li>
</ul>

<h3>Modelos de Implementação (Execução do Programa)</h3>

<p>O processo de rodar um programa pode ocorrer de três formas:</p>

<ul>
  <li>
    <strong>Compilação:</strong> Transforma o código escrito diretamente em linguagem
    de máquina para execução. Após a compilação, não é necessário outro programa
    para rodá-lo.
  </li>
  <li>
    <strong>Interpretação Pura:</strong> O código é interpretado diretamente por
    outro programa dedicado durante a execução. Comum em programas de cálculo iterativo
    de engenharia, como MATLAB e Maple.
  </li>
  <li>
    <strong>Sistemas Híbridos:</strong> Realizam uma mistura entre os processos de
    compilação e interpretação.
  </li>
</ul>

<h4>Elementos Auxiliares de Implementação</h4>

<ul>
  <li>
    <strong>Pré-processador:</strong> Programa que processa o código e organiza tarefas/procedimentos
    imediatamente antes de realizar a compilação.
  </li>
  <li>
    <strong>Ambiente de Programação (IDE):</strong> Sigla para Integrated Development
    Environment (Ambiente de Desenvolvimento Integrado). É o conjunto de ferramentas
    aplicadas no desenvolvimento de softwares, utilizado para escrever códigos, compilar
    e depurar (debugar) erros.
  </li>
</ul>

<h3>Índice TIOBE</h3>

<p>
  O Índice TIOBE é um indicador mensal de popularidade das linguagens de
  programação, calculado com base na frequência de pesquisas em websites da
  internet. O índice indica popularidade, mas não deve ser usado como o único
  indicador de sucesso de uma linguagem, pois depende de fatores externos além
  da dificuldade ou aplicabilidade técnica.
</p>

<h3>Sentença, Sintaxe e Semântica</h3>

<p>
  A definição e a estruturação de uma linguagem de programação dependem de três
  conceitos fundamentais que determinam como o código é escrito e interpretado:
</p>

<ul>
  <li>
    <strong>Sentença:</strong> É uma cadeia de caracteres elaborada com base em
    um alfabeto. Na prática, representa os passos de execução de um algoritmo ou
    as declarações de variáveis distribuídas nas linhas do programa (equivalente
    a um ingrediente ou a uma instrução individual em uma receita).
    <ul>
      <li>
        <strong>Particularidades:</strong> Em linguagens de baixo nível como Assembly,
        cada sentença deve ocupar uma linha própria. Em linguagens como C, as sentenças
        são obrigatoriamente encerradas com ponto e vírgula (;), permitindo que mais
        de uma instrução ocupe a mesma linha.
      </li>
    </ul>
  </li>
  <li>
    <strong>Sintaxe:</strong> Refere-se à forma e à estrutura das expressões, sentenças
    e unidades do programa. É a regra de "como" cada sentença deve ser escrita e
    organizada. Alterar a ordem, omitir ou adicionar elementos fora do padrão viola
    a sintaxe e impede a execução correta do algoritmo.
  </li>
  <li>
    <strong>Semântica:</strong> Diz respeito ao significado das sentenças, expressões
    e unidades do programa. É a definição de "o que a sentença faz" ou "o que ela
    quer dizer" ao ser executada pelo sistema.
  </li>
</ul>

<p>
  A sintaxe e a semântica possuem finalidades separadas, mas são fortemente
  relacionadas, pois juntas fornecem sentido prático a elementos abstratos.
</p>

<h3>Lexemas e Tokens</h3>

<p>
  Durante o processo de compilação, a estrutura do código é dividida em unidades
  fundamentais:
</p>

<ul>
  <li>
    <strong>Lexema:</strong> É a descrição formal da sintaxe, representando a unidade
    sintática mais elementar da linguagem (a sequência de caracteres exatamente como
    é digitada no código).
  </li>
  <li>
    <strong>Token:</strong> É a categoria ou identificador abstrato usado para caracterizar
    e classificar um lexema.
  </li>
</ul>

<h4>Exemplos de Correspondência</h4>

<ul>
  <li>
    Tipo de Token
    <ul>
      <li>Plavras-chave</li>
      <li>Identificadores</li>
      <li>Constantes</li>
      <li>Sinais/Operadores</li>
    </ul>
  </li>
  <li>
    Exemplo de Lexema
    <ul>
      <li>begin, integer</li>
      <li>a, var1</li>
      <li>421, 7.6E4</li>
      <li>+, &lt;=</li>
    </ul>
  </li>
</ul>

<p>
  A coleção dessas regras de escrita de uma linguagem forma a sua gramática
  (também conhecida como descrição BNF).
</p>

<h3>Classificações da Semântica</h3>

<p>
  A semântica busca explicar o significado dos códigos de maneira unívoca,
  eliminando ambiguidades. Ela se divide em quatro categorias:
</p>

<ul>
  <li>
    <strong>Semântica Dinâmica:</strong> Trata do significado das expressões, sentenças
    e unidades de programa diretamente na escrita do código.
  </li>
  <li>
    <strong>Semântica Operacional:</strong> Discorre sobre o significado de uma sentença
    ou programa com base nos efeitos e alterações que eles geram na máquina no momento
    da execução.
  </li>
  <li>
    <strong>Semântica Denotacional:</strong> É o método mais rigoroso de descrição
    de programas. Baseia-se na definição de um objeto matemático específico e de
    uma função para mapear as instâncias e entidades da linguagem.
  </li>
  <li>
    <strong>Semântica Axiomática:</strong> Baseada na lógica matemática, possui caráter
    abstrato. Não especifica o significado direto do programa, mas define o que pode
    ser formalmente provado sobre ele.
  </li>
</ul>

<h3>Análise Léxica e Análise Sintática</h3>

<p>
  No processo de compilação ou interpretação dentro de uma IDE, a verificação do
  código baseia-se na descrição da sintaxe formal da linguagem. Essa tarefa é
  dividida em duas etapas sequenciais:
</p>

<h4>Analisador Léxico</h4>

<ul>
  <li>
    Atua como um casador de padrões e representa a primeira fase da compilação.
  </li>
  <li>
    Sua função é isolar pequenos lexemas para avaliação, detectando se há
    caracteres ou palavras escritas incorretamente no código.
  </li>
  <li>
    <strong>Analogia:</strong> Funciona de forma semelhante ao sublinhado vermelho
    de erro ortográfico em editores de texto.
  </li>
</ul>

<h4>Analisador Sintático</h4>

<ul>
  <li>Entra em ação após a análise léxica.</li>
  <li>
    Seu objetivo é detectar erros sintáticos e construir uma árvore de análise
    sintática.
  </li>
  <li>
    Analisa a fundo como os lexemas se relacionam e se estruturam entre si no
    programa.
  </li>
  <li>
    <strong>Analogia:</strong> Equivale ao sublinhado azul de erro gramatical/estrutural
    em editores de texto (quando as palavras estão corretas isoladamente, mas a relação
    entre elas está incorreta).
  </li>
</ul>

<h3>Conclusão: Conceitos-Chave</h3>

<p>
  O fechamento desta etapa reforça os critérios essenciais para a escolha,
  classificação e funcionamento das linguagens de programação:
</p>

<ul>
  <li>
    <strong>Inexistência de uma linguagem soberana:</strong> Não há uma linguagem
    de programação universalmente melhor. A escolha ideal depende estritamente da
    aplicação desejada e da facilidade de programação.
  </li>
  <li>
    <strong>Relação entre os critérios de escolha:</strong>
    <ul>
      <li>
        <strong>Legibilidade:</strong> É influenciada diretamente pelo número de
        construções, recursos e operadores da linguagem.
      </li>
      <li>
        <strong>Capacidade de Escrita:</strong> Quanto mais fácil e abstrata for
        a linguagem, mais simples se torna o ato de programar.
      </li>
      <li>
        <strong>Confiabilidade:</strong> Programas escritos em linguagens fáceis
        de ler e de escrever tornam-se naturalmente mais confiáveis.
      </li>
      <li>
        <strong>Custo:</strong> O custo financeiro e de tempo é um reflexo direto
        de todos os fatores anteriores (legibilidade, escrita e confiabilidade).
      </li>
    </ul>
  </li>
  <li>
    <strong>Categorias e Popularidade:</strong> As linguagens dividem-se em quatro
    categorias: imperativas (as mais populares), funcionais, lógicas e de marcação/híbridas.
    A popularidade de cada uma na web é mensurada e listada pelo Índice TIOBE.
  </li>
  <li>
    <strong>Sintaxe vs. Semântica:</strong>
    <ul>
      <li>
        <strong>Sintaxe:</strong> Define a forma das expressões (o formato exato
        do que se escreve).
      </li>
      <li>
        <strong>Semântica:</strong> Define o significado das expressões (o propósito
        ou para que se escreve).
      </li>
      <li>
        Ambas fornecem a base estrutural para o funcionamento dos analisadores
        léxicos, sintáticos e semânticos na criação de compiladores.
      </li>
    </ul>
  </li>
</ul>
