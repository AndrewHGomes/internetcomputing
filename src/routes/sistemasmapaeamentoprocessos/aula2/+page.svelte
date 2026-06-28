<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Modelagem de Processos</h2>

<Audios modulo="M13" aulas={["05", "06", "07", "08"]} />

<p>
  A modelagem de processos de negócios é o ponto de partida para alinhar uma
  organização e melhorar suas operações. Nenhuma empresa opera no nível ideal
  desde o início; atingir o funcionamento ideal exige tempo, reflexão e esforço.
  O foco deve ser a melhoria contínua, com equipes preparadas para analisar e
  corrigir processos constantemente.
</p>

<h3>O que é e por que modelar?</h3>

<p>
  Cada negócio possui objetivos próprios em seu setor. A modelagem ajuda as
  equipes a refletirem sobre como uma tarefa é executada e como pode melhorar.
  Ao descrever um processo, fica mais fácil identificar áreas problemáticas e
  inconsistências. A representação gráfica dos processos serve para aumentar a
  compreensão e a eficiência geral do negócio, permitindo visualizar melhor as
  interações com os clientes e identificar oportunidades de melhoria. Processos
  aprimorados tornam a empresa mais eficaz, produtiva e lucrativa.
</p>

<h4>Benefícios da Modelagem de Processos</h4>

<ul>
  <li>
    <strong>Alinhamento operacional e estratégico:</strong> Garante que as operações
    da empresa estejam alinhadas à sua estratégia geral.
  </li>
  <li>
    <strong>Consistência e padronização:</strong> Identifica os melhores processos
    para que sejam padronizados e usados de forma consistente em toda a aplicação.
  </li>
  <li>
    <strong>Comunicação aprimorada:</strong> Melhora a comunicação interna e ajuda
    a manter o fluxo de processos em momentos de mudanças.
  </li>
  <li>
    <strong>Transparência e responsabilidade:</strong> Dissemina a conscientização
    e aumenta a transparência e a responsabilidade entre os colaboradores.
  </li>
  <li>
    <strong>Agilidade do processo:</strong> Prepara a empresa para mudanças, especialmente
    as que envolvem integração e avanços tecnológicos.
  </li>
  <li>
    <strong>Capacidade de competir:</strong> Permite competir e sobreviver no mercado
    por meio da dedicação de tempo e realização das alterações necessárias.
  </li>
</ul>

<h4>Níveis de Evolução e Abordagem "Como Está" (As-Is)</h4>

<p>
  O processo de modelagem normalmente evolui em três etapas: começa por um
  <strong>diagrama de processos</strong>, evolui para um <strong>mapa</strong>
  e, por fim, define-se o <strong> modelo de processos </strong>. Os princípios
  básicos de um projeto de modelagem incluem:
</p>

<ol>
  <li>
    <strong>Modelo "no estado em que se encontra" (As-Is):</strong> Descreve as operações
    e processos atuais da maneira mais refinada possível, seja no papel ou em um
    software.
  </li>
  <li>
    <strong>Revisão e análise:</strong> Utiliza o modelo atual para identificar processos
    ineficazes, inconsistências e problemas no atingimento de metas operacionais.
    As características e a finalidade do ambiente afetam esse desenvolvimento.
  </li>
  <li>
    <strong>Modelo potencial (To-Be):</strong> Definição de como as operações podem
    melhorar e se tornar mais eficientes.
  </li>
</ol>

<h4>BPM (Business Process Management)</h4>

<p>
  O BPM é a forma mais eficaz de melhorar os processos porque envolve análise e
  aprimoramento contínuo. As melhores empresas trabalham constantemente nisso,
  pois sempre há espaço para melhorias.
</p>

<h3>Fluxos de Trabalho (Workflows)</h3>

<p>
  Os fluxos de trabalho são utilizados para desenvolver determinados processos,
  rastreando todas as tarefas executadas de forma manual e automática, além de
  descreverem as informações necessárias para cada parte. Sua abordagem pode ser
  muito rígida, sendo criticada pela inflexibilidade. De acordo com a ABPMP
  (2014), os modelos são produzidos para representar e ilustrar tanto o fluxo de
  trabalho da situação atual quanto o do estado futuro (que visa modificações
  para maior qualidade ou produtividade). Processos caóticos — caracterizados
  por fluxos de trabalho longos, sinuosos e com entrecruzamento de atividades —
  provocam prolongados tempos de espera e retrabalho. Dentro do contexto amplo
  do BPM, encontram-se ferramentas voltadas para a modelagem, monitoramento,
  automação e simulação de processos.
</p>

<h3>Técnicas de Mapeamento Eficaz</h3>

<p>
  Não existe uma única maneira de modelar processos. Há diferentes meios de
  mapear e documentar o fluxo utilizando auxílios visuais.
</p>

<h4>Técnica de Fluxo de Trabalho</h4>

<p>
  Essa técnica é usada para mapear fluxos de tarefas por pessoas. O objetivo é
  identificar todos os detalhes importantes de cada tarefa, que podem fluir de
  várias maneiras. O exemplo do fluxo de venda de ingresso para o cliente
  demonstra essa aplicação em etapas sequenciais:
</p>

<ol>
  <li>O processo inicia com a chegada do cliente no cinema.</li>
  <li>O cliente informa os dados da sessão a que deseja assistir.</li>
  <li>O atendente verifica a disponibilidade do ingresso.</li>
  <li>
    Se não existir ingresso disponível, o processo se encerra e o ingresso não é
    entregue.
  </li>
  <li>
    Se existir ingresso disponível, o cliente verifica se tem dinheiro para
    pagar.
  </li>
  <li>
    Se o cliente não tiver dinheiro o suficiente, o processo se encerra e o
    ingresso não é entregue.
  </li>
  <li>Se o cliente tiver dinheiro, paga pelo ingresso.</li>
  <li>O balconista entrega o ingresso para o cliente.</li>
  <li>O processo encerra com o ingresso entregue.</li>
</ol>

<h4>Técnica de Fluxograma</h4>

<p>
  É uma das técnicas mais antigas para descrever processos e é facilmente
  compreendida. Os fluxogramas utilizam poucos símbolos para descrever as ações
  de cada parte do negócio até o final do processo. O ideal para uma empresa é
  possuir uma ferramenta de fluxo de trabalho que seja multifuncional e
  flexível, permitindo gerenciar processos, portfólio, projetos, CRM, P&D, entre
  outras áreas.
</p>

<h3>Diagramas como Auxílio para Mapear Processos</h3>

<p>
  Muitas empresas utilizam representações gráficas baseadas na Business Process
  Modeling Notation (BPMN) para facilitar o entendimento dos papéis e das
  responsabilidades de todos os envolvidos. Esses diagramas acompanham entradas,
  saídas, objetivos e demais elementos do processo.
</p>

<h4>Tipos de Diagramas e Métodos</h4>

<ul>
  <li>
    <strong>Diagramas de Fluxo de Dados (DFD):</strong> Monitoram o fluxo de dados
    brutos do cliente e da empresa para atingir o resultado desejado. Apresentam
    quatro símbolos, e cada processo possui duas características: um número de identificação
    e um nome.
  </li>
  <li>
    <strong>Gráficos de Gantt:</strong> Colocam as tarefas em uma escala de tempo
    para descrever cada etapa e o tempo ideal projetado para a conclusão, representando
    o cronograma do projeto.
  </li>
  <li>
    <strong>Diagramas de Atividades por Funções:</strong> Usados para descrever os
    comportamentos desejados, destacando-se como um dos modelos mais simples de ler.
    Permitem acrescentar detalhes iniciais (como ID de usuário e senha) para limitar
    tentativas de acesso.
  </li>
  <li>
    <strong>Diagrama de Atividades UML:</strong> Método orientado a objetos utilizado
    principalmente para desenvolver sistemas de software e estruturar a lógica de
    um processo de negócios.
  </li>
  <li>
    <strong>Diagramas de Interação:</strong> Identificam as funções desempenhadas
    pelo cliente e pelos departamentos da empresa para concluir as atividades de
    um processo. Apresentam maior complexidade que outros modelos, mas oferecem flexibilidade.
  </li>
  <li>
    <strong>Redes de Petri:</strong> Aplicadas em processos mais complexos. Existem
    em várias formas e são compostas por locais ($P$) e transições ($t$), diferenciando
    cada rede de processos.
  </li>
</ul>

<h3>Métodos Orientados a Objetos e Simulação</h3>

<h4>Métodos Orientados a Objetos</h4>

<p>
  Neste método, objetos e grupos de objetos (classes) são documentados por um
  engenheiro de software à medida que seus estados mudam de acordo com o
  comportamento deles diante dos dados extraídos do cliente. Objetos são
  entidades de modelagem de sistemas que armazenam estados utilizando seus
  atributos e interagem entre si por meio da troca de mensagens (Engholm, 2017).
  Eles são classificados em:
</p>

<ul>
  <li><strong>Ator:</strong> Solicita e recebe serviços (objeto-cliente).</li>
  <li>
    <strong>Servidor:</strong> Presta serviços a outros objetos do sistema.
  </li>
  <li><strong>Agente:</strong> Atua tanto como ator quanto como servidor.</li>
</ul>

<h4>Simulação</h4>

<p>
  Utilizada quando os processos são altamente complexos, servindo para entender
  melhor como eles operariam no mundo real. Cada método possui a capacidade de
  esclarecer objetivos e aprimorar processos, cabendo a cada empresa considerar
  qual deles funciona melhor para seus propósitos específicos.
</p>

<h3>Mapeamento vs. Modelagem de Processos</h3>

<ul>
  <li>
    <strong>Mapeamento:</strong> É mais amplo; serve para identificar todos os departamentos
    e funcionários envolvidos.
  </li>
  <li>
    <strong>Modelagem:</strong> É mais focada nos detalhes dos processos; serve para
    aumentar a eficiência por meio da análise de serviços e resultados.
  </li>
</ul>

<p>
  A modelagem (BPM) funciona como a representação dos processos de negócio de
  uma organização para fins de documentação, entendimento e análise, permitindo
  sua transformação e automatização.
</p>

<h3>Tipos de Técnicas de Modelagem</h3>

<p>
  Toda técnica exige a análise das operações, um responsável pela revisão e um
  modelo de processo a ser seguido. As principais possibilidades são:
</p>

<ul>
  <li>
    <strong>Modelo de Processo de Negócios e Notação (BPMN):</strong> Projetado para
    facilitar o entendimento. Consiste em objetos de fluxo (eventos, atividades e
    gateways), setas que indicam o fluxo (de sequências, mensagens e associações)
    e artefatos (objetos de dados, grupos e anotações).
  </li>
  <li>
    <strong>Linguagem de Modelagem de Ciclo de Vida (LML):</strong> Trata-se de um
    sistema complexo de operação. Usada para capturar informações ao longo do ciclo
    de vida dos processos por meio de diagramas para todas as classes (ação, ativo,
    interface, hierarquia, hora, local, definição de classe, diagramas físicos e
    funcionais combinados, gráficos de risco, organização, barra e linha).
  </li>
  <li>
    <strong>Gerenciamento de Processos de Negócios Orientado ao Assunto:</strong
    > Focado no sujeito/assunto como a parte mais influente do processo. Estrutura-se
    conforme o papel de cada sujeito no processo geral para melhorar a rede de comunicação
    entre as partes e fornecer uma estrutura fácil de entender.
  </li>
  <li>
    <strong>Linguagem de Modelagem de Negócios Estendida:</strong> Linguagem gráfica
    intuitiva utilizada para projetar diagramas com base nos fatores organizacionais:
    "quem", "o quê", "qual", "quando" e "onde".
  </li>
  <li>
    <strong>Cadeia de Processos Orientada a Eventos:</strong> Baseia-se em fluxogramas
    e utiliza gráficos para mostrar o fluxo de eventos através dos processos. É aplicada
    no planejamento de recursos e no delineamento de melhorias.
  </li>
  <li>
    <strong>Linguagem de Modelagem Unificada (UML):</strong> Abordagem orientada
    a objetos com diversos tipos de diagramas, utilizada para analisar a lógica dos
    processos.
  </li>
  <li>
    <strong>Notação Administrativa Formalizada:</strong> Usada para implementar softwares
    de planejamento de recursos e de melhoria no relacionamento com os clientes,
    visando aumentar a sistematização.
  </li>
</ul>

<p>
  Dominar todos os símbolos das notações pode ser difícil, mas compreender os
  conceitos auxilia no entendimento. Empresas que não sabem por onde iniciar a
  modelagem podem contratar organizações especializadas ou adquirir softwares
  específicos de modelagem de processos.
</p>

<h3>Agregação de Valor nos Processos</h3>

<p>
  A análise das operações e atividades de uma empresa busca torná-la mais
  eficiente e produtiva, diminuindo gargalos, atrasos e desperdícios. Para isso,
  é fundamental pensar em agregar valor para o cliente e para o negócio. No
  contexto de gestão de cursos e orçamento, o valor agregado é definido como uma
  avaliação entre o que foi obtido em relação ao que foi gasto e ao que se
  planejava gastar. Propõe-se que o valor a ser agregado inicialmente por uma
  atividade é o valor orçado para ela (Viana, 2018).
</p>

<h3>Diretrizes para Desenvolver Bons Modelos de Processo</h3>

<p>
  Após alinhar o foco na agregação de valor, o desenvolvimento de um bom modelo
  deve seguir estas práticas:
</p>

<ul>
  <li>
    <strong>Planejamento e Recursos:</strong> Entender os benefícios da modelagem,
    pensar em níveis funcionais de processos, identificar recursos de ajuda e adquirir
    todos os documentos e formulários logo no início.
  </li>
  <li>
    <strong>Metas e Regras:</strong> Identificar as metas necessárias para os modelos
    de processo, documentar as regras do negócio e vinculá-las a esses modelos.
  </li>
  <li>
    <strong>Detalhamento Técnico:</strong> Documentar tudo, detalhar as etapas dos
    processos individuais, destacar as saídas de cada etapa e diferenciar quais etapas
    são manuais e quais são automáticas.
  </li>
  <li>
    <strong>Prazos e Fluxos:</strong> Desenvolver listas de tarefas com o tempo necessário
    para sua conclusão e validar a forma como cada processo flui.
  </li>
  <li>
    <strong>Identificação e Rótulos:</strong> Rotular todas as partes (especialmente
    início e fim), criar rótulos adequados para o tipo de ação, identificar o resultado
    de cada processo e utilizar uma grade (colunas e linhas) ou painel esquerdo para
    identificar cargos e funções.
  </li>
  <li>
    <strong>Notação e Simbologia:</strong> Escolher uma notação clara, definir os
    símbolos utilizados, manter uma chave (legenda) para eles no modelo e certificar-se
    de que todas as etapas avancem o processo.
  </li>
  <li>
    <strong>Simplicidade e Alternativas:</strong> Detalhar rotas alternativas, reutilizar
    elementos do modelo quando possível, escolher as ferramentas certas e evitar
    a complexidade excessiva usando poucos elementos.
  </li>
  <li>
    <strong>Tecnologia:</strong> Considerar o uso de um software BPM apropriado que
    se adapte às necessidades de modelagem da empresa.
  </li>
</ul>

<h3>Conclusão</h3>

<ul>
  <li>
    <strong>Modelagem de Processos:</strong> Permite a representação dos processos
    da empresa em forma de modelos por meio da aplicação de metodologias e técnicas
    conhecidas.
  </li>
  <li>
    <strong>Fluxo de Trabalho (Workflow):</strong> Sua aplicação serve para garantir
    que o capital humano atue de forma efetiva, buscando a produtividade de maneira
    adequada e otimizada.
  </li>
  <li>
    <strong>Diagramas no Mapeamento:</strong> Funcionam como ferramentas de auxílio
    que facilitam a visualização da ordem, dos custos, do tempo e das demais características
    identificadas durante o mapeamento de processos.
  </li>
  <li>
    <strong>Técnicas de Modelagem:</strong> São aplicadas por empresas que buscam
    a padronização. Elas fornecem instrumentos visuais intuitivos, criam fluxogramas
    e diagramas, simulam processos e auxiliam o usuário no entendimento das conexões
    de cada objeto.
  </li>
  <li>
    <strong>Desenvolvimento de Bons Modelos:</strong> Viabiliza o processo organizacional,
    ajudando a monitorar e a otimizar as operações em busca de melhoria contínua,
    aumento da eficiência e redução de custos.
  </li>
</ul>
