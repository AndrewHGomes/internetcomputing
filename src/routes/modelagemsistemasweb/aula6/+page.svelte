<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Introdução à Modelagem UML Complementar</h2>

<Audios modulo="M8" aulas={["21", "22", "23", "24"]} />

<p>
  A modelagem de um sistema de software exige diferentes perspectivas para
  garantir a qualidade técnica e o atendimento aos requisitos. Enquanto os
  diagramas de <strong>Casos de Uso</strong> e de <strong>Classes</strong> são fundamentais
  e onipresentes, outros diagramas são aplicados conforme a necessidade específica
  do projeto para agregar valor ao entendimento do todo. Nesta etapa, o foco recai
  sobre diagramas que capturam aspectos dinâmicos e comportamentais do software,
  sendo eles:
</p>

<ul>
  <li>Diagrama de Estados.</li>
  <li>Diagrama de Atividades.</li>
  <li>Diagrama de Sequência.</li>
</ul>

<h3>O Diagrama de Estado</h3>

<p>
  O <strong>Diagrama de Estado</strong> (também chamado de Máquina de Estados ou
  Transição de Estados) é um diagrama dinâmico que descreve o comportamento de um
  objeto ao longo de seu ciclo de vida. Ele detalha como um objeto evolui em resposta
  a eventos específicos dentro do sistema.
</p>

<h4>Características e Uso</h4>

<ul>
  <li>
    <strong>Objetivo:</strong> Representar os estados possíveis de um objeto e as
    transições causadas por eventos.
  </li>
  <li>
    <strong>Aplicação:</strong> Deve ser utilizado quando há complexidade na transição
    de estados de objetos críticos para o negócio.
  </li>
  <li>
    <strong>Base de Construção:</strong> Apoia-se na descrição dos Casos de Uso e
    no Diagrama de Classes para mostrar as mudanças de comportamento.
  </li>
</ul>

<h4>Conceitos Fundamentais</h4>

<p>
  A transição de estado é o ponto central deste diagrama. Um exemplo clássico é
  o de um telefone analógico:
</p>

<ul>
  <li><strong>Estados possíveis:</strong> Ocioso ou Ativo/Ocupado.</li>
  <li>
    <strong>Evento de mudança:</strong> A ação de "tirar do gancho" ou "colocar no
    gancho" é o que determina a transição entre os estados.
  </li>
</ul>

<p>
  O diagrama, portanto, mapeia exatamente essas condições (estados) e os
  gatilhos (eventos) que fazem o objeto mudar de uma condição para outra.
</p>

<h3>Elementos do Diagrama de Estado</h3>

<p>
  O Diagrama de Estado descreve a dinâmica de um objeto através de quatro
  elementos fundamentais, que detalham como e por que uma mudança de
  comportamento ocorre.
</p>

<h4>Objeto</h4>

<p>
  É o elemento central da modelagem, representando a entidade que sofre as
  alterações de comportamento ao longo do ciclo de vida no sistema (ex: um
  pedido, uma conta bancária ou um aparelho telefônico).
</p>

<h4>Estado</h4>

<p>
  Representa a condição ou situação de um objeto em um momento específico,
  compreendido entre dois eventos. O objeto permanece em um estado até que um
  novo estímulo provoque uma mudança.
</p>

<h4>Evento</h4>

<p>
  É o gatilho ou ocorrência que dispara uma mudança de estado. Os eventos podem
  ser classificados em três tipos:
</p>

<ul>
  <li>
    <strong>Externo:</strong> Gerado por atores ou sistemas fora do limite do software
    (ex: clique do usuário).
  </li>
  <li>
    <strong>Interno:</strong> Gerado por elementos dentro do próprio sistema (ex:
    comunicação entre objetos).
  </li>
  <li>
    <strong>Temporal:</strong> Disparado por uma data, hora específica ou decorrer
    de um intervalo de tempo.
  </li>
</ul>

<h4>Transição</h4>

<p>
  É o relacionamento que conecta dois estados. Ela indica o caminho que o objeto
  percorre para sair de um estado anterior e entrar em um novo após a ocorrência
  de um evento.
</p>

<p>
  <strong>Observação sobre a Prática:</strong> A modelagem de estados deve ser aplicada
  criteriosamente. Se a transição de um objeto for simples ou óbvia, o esforço da
  modelagem pode não trazer benefícios. O diagrama é recomendado apenas quando agrega
  clareza a processos complexos, evitando desperdício de tempo e recursos.
</p>

<h3>Diagrama de Atividades</h3>

<p>
  O <strong>Diagrama de Atividades</strong> foca no fluxo de controle entre ações.
  Ele descreve a lógica de uma funcionalidade, de um processo de negócio ou de um
  fluxo de trabalho, funcionando como a representação da UML para processos automatizados.
  Sua função é decompor um processo para entender quais atividades são sequenciais,
  concorrentes ou paralelas.
</p>

<h4>Elementos do Diagrama</h4>

<p>
  Para construir a lógica de um fluxo, utilizam-se os seguintes componentes:
</p>

<ul>
  <li>
    <strong>Estado Inicial e Final:</strong> Indicam, respectivamente, onde o processo
    começa e onde ele termina. Um diagrama possui ao menos um de cada.
  </li>
  <li>
    <strong>Atividades:</strong> Representam as ações ou tarefas a serem executadas.
    São desenhadas como retângulos com bordas arredondadas.
  </li>
  <li>
    <strong>Transição:</strong> Representada por setas contínuas, indica o caminho
    e a ordem de execução das atividades.
  </li>
  <li>
    <strong>Decisões:</strong> Representadas por um losango, servem para criar desvios
    no fluxo baseados em expressões lógicas (condicionais).
  </li>
  <li>
    <strong>Bifurcação (Fork) e União (Join):</strong> Representadas por uma barra
    sólida. A bifurcação divide o fluxo em atividades paralelas, enquanto a união
    sincroniza esses fluxos múltiplos de volta em um único caminho.
  </li>
</ul>

<h4>Exemplo Prático: Construção de uma Casa</h4>

<p>O diagrama organiza as etapas de forma lógica:</p>

<ol>
  <li><strong>Início:</strong> Seleção do local.</li>
  <li>
    <strong>Sequência:</strong> Contratação de arquiteto → Elaboração da planta →
    Orçamento do construtor.
  </li>
  <li>
    <strong>Execução:</strong> Após aprovação financeira, iniciam-se as atividades
    práticas (licenças, fundação, estrutura).
  </li>
  <li>
    <strong>Fim:</strong> Entrega das chaves e documentação ao proprietário.
  </li>
</ol>

<p>
  Mesmo em processos complexos, o diagrama simplifica a visão técnica ao
  transformar o passo a passo em uma sequência visual clara.
</p>

<h3>Diagrama de Sequência</h3>

<p>
  O <strong>Diagrama de Sequência</strong> é uma ferramenta da UML que descreve como
  os objetos de um sistema interagem entre si para realizar uma tarefa específica.
  Ele detalha a ordem temporal das mensagens trocadas, focando na lógica de execução
  de uma transação.
</p>

<h4>Estrutura do Diagrama</h4>

<p>O diagrama é organizado em duas dimensões principais:</p>

<ul>
  <li>
    <strong>Dimensão Horizontal:</strong> Representa os objetos ou atores envolvidos
    na interação (ex: Cliente, Sistema, Banco de Dados).
  </li>
  <li>
    <strong>Dimensão Vertical:</strong> Representa a passagem do tempo, indicando
    quando cada ação ocorre e a duração da vida de um objeto durante aquele processo.
  </li>
</ul>

<h4>Elementos Centrais</h4>

<ul>
  <li>
    <strong>Linhas de Vida (Lifelines):</strong> Representam a existência de um objeto
    ao longo do tempo. Elas mostram quando um objeto está ativo, quando é criado
    e quando é destruído.
  </li>
  <li>
    <strong>Mensagens:</strong> São as setas que ligam as linhas de vida, representando
    a comunicação ou solicitação de serviço entre os objetos.
  </li>
  <li>
    <strong>Estruturas de Controle:</strong> Definem a lógica da interação, como
    loops ou condições, determinando quais mensagens são enviadas em quais cenários.
  </li>
</ul>

<h4>Exemplo de Aplicação</h4>

<p>
  Em um cenário bancário, o diagrama de sequência mapearia a interação entre um
  <strong>Cliente</strong>, um <strong>Funcionário</strong> e o
  <strong>Sistema do Banco</strong>:
</p>

<ol>
  <li>O Cliente solicita uma operação (mensagem).</li>
  <li>O Funcionário valida os dados no Sistema (mensagem entre objetos).</li>
  <li>O Sistema retorna a confirmação (mensagem de resposta).</li>
</ol>

<h3>Elementos do Diagrama de Sequência</h3>

<p>
  O Diagrama de Sequência detalha a troca de informações entre componentes. Para
  sua construção, utiliza-se como base os <strong>Requisitos</strong> e os
  <strong>Casos de Uso</strong>, garantindo que a visão técnica esteja alinhada
  à necessidade do negócio.
</p>

<h4>Componentes Principais</h4>

<ul>
  <li>
    <strong>Ator:</strong> O usuário ou sistema externo que inicia a interação e
    a troca de mensagens.
  </li>
  <li>
    <strong>Linha de Vida:</strong> Representada por uma linha pontilhada vertical,
    indica a existência de um objeto/componente durante o processo, desde sua criação
    até sua destruição.
  </li>
  <li>
    <strong>Mensagem:</strong> Representada por setas que indicam a direção do fluxo,
    é a informação ou comando que trafega entre as linhas de vida.
  </li>
  <li>
    <strong>Fragmento:</strong> Retângulos que envolvem partes do fluxo para representar
    estruturas lógicas, como condicionais (if/else) ou repetições (for/while).
  </li>
  <li>
    <strong>Caixa de Ativação:</strong> Indica o período em que um objeto está executando
    uma operação ou método.
  </li>
</ul>

<h4>Exemplo Prático e Aplicação</h4>

<p>
  Em um cenário de vendas envolvendo os objetos <strong>Pedido</strong> e
  <strong>Estoque</strong>:
</p>

<ol>
  <li>
    O <strong>Ator (Vendedor)</strong> inicia o processo enviando uma mensagem.
  </li>
  <li>
    O objeto <strong>Pedido</strong> é criado, executa seus métodos (ações) e
    interage com o
    <strong>Estoque</strong>.
  </li>
  <li>
    As <strong>Linhas de Vida</strong> mostram exatamente onde cada objeto nasce
    e onde é finalizado (destruído) após cumprir sua função.
  </li>
</ol>

<h3>Utilidade</h3>

<p>
  Este diagrama é indispensável em softwares com <strong
    >troca intensa de informações</strong
  >, pois permite rastrear o caminho completo de um dado, identificando todos os
  objetos e métodos acionados desde o início até a conclusão da transação.
</p>

<h3>Conclusão: O Papel da UML na Qualidade do Software</h3>

<p>
  A <strong>UML (Unified Modeling Language)</strong> consolida-se como a
  linguagem universal para análise e projeto de sistemas, fornecendo uma notação
  precisa que transcende metodologias, sendo aplicada tanto em contextos
  <strong>tradicionais</strong>
  quanto <strong>ágéis</strong>.
</p>

<h4>Diretrizes para o Analista de Sistemas</h4>

<ul>
  <li>
    <strong>Valor Agregado:</strong> O analista deve selecionar apenas os diagramas
    que realmente contribuem para o entendimento do sistema. Não é necessário utilizar
    todos os diagramas da UML em todos os projetos.
  </li>
  <li>
    <strong>Documentação Just-in-Time:</strong> Seguindo princípios ágeis, a documentação
    deve ser a estritamente necessária e fundamental para a construção do software.
    Documentar além do necessário é considerado desperdício.
  </li>
  <li>
    <strong>Foco no Cliente:</strong> O objetivo final da modelagem não é apenas
    a técnica, mas garantir que o software atenda às necessidades do cliente com
    a melhor solução técnica possível.
  </li>
</ul>
