<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Análise Essencial: Conceito e Fundamentos</h2>

<Audios modulo="M12" aulas={["13", "14", "15", "16"]} />

<p>
  A <strong>Análise Essencial</strong> é um conjunto de técnicas voltado para a
  definição de sistemas com foco total na <strong>essência do negócio</strong>.
  Sua premissa fundamental é a abstração tecnológica: projeta-se o sistema
  ignorando restrições de hardware, software, custos ou falhas. Considera-se um
  "ambiente tecnológico perfeito", com processamento instantâneo e memória
  infinita, para garantir que o desenho do software atenda estritamente às
  necessidades da organização, independentemente de como será implementado.
</p>

<p>
  Diferente de outras abordagens, a Análise Essencial parte do princípio de que
  a lógica de um negócio existe por si só, e o computador é apenas uma
  ferramenta posterior. O objetivo é capturar a ideia central e o argumento
  principal do sistema antes de qualquer automação.
</p>

<h3>Componentes e Modelagem</h3>

<p>
  A estrutura da Análise Essencial divide-se em duas frentes principais que
  definem o escopo e o funcionamento do sistema:
</p>

<ul>
  <li>
    <strong>Modelo Ambiental:</strong> Estabelece os limites e fronteiras entre o
    sistema e o mundo externo.
  </li>
  <li>
    <strong>Modelo Comportamental:</strong> Descreve as operações internas e como
    o sistema reage para interagir com o ambiente.
  </li>
  <li>
    <strong>Métodos Utilizados:</strong> Baseia-se na modelagem de dados e na modelagem
    funcional, reagindo a eventos externos para gerar respostas específicas do sistema.
  </li>
</ul>

<h4>Diferenças: Análise Essencial vs. Análise Estruturada</h4>

<p>
  A Análise Essencial começa pelo modelo essencial e pela ideia central,
  enquanto a Análise Estruturada inicia diretamente pelo modelo lógico proposto.
  Quanto às perspectivas, a Essencial aborda função, dados e controle, com
  particionamento por eventos. Já a Estruturada foca apenas em função e dados,
  utilizando a abordagem top-down.
</p>

<h3>Introdução à Análise Orientada a Objetos (AOO)</h3>

<p>
  A <strong>Análise Orientada a Objetos</strong> surge como uma evolução nas técnicas
  de desenvolvimento, focando na organização do sistema através de elementos do mundo
  real. Seus conceitos fundamentais incluem:
</p>

<ul>
  <li>
    <strong>Objetos e Classes:</strong> Representações de entidades e suas categorias.
  </li>
  <li>
    <strong>Atributos:</strong> Características ou dados que definem o objeto.
  </li>
  <li>
    <strong>Métodos:</strong> Comportamentos ou ações que os objetos podem executar.
  </li>
</ul>

<p>
  O foco da AOO é integrar esses elementos para melhorar a qualidade do
  desenvolvimento, reaproveitando técnicas preexistentes e aplicando as
  evoluções necessárias para sistemas modernos.
</p>

<h3>Componentes da Análise Essencial</h3>

<p>
  A Análise Essencial divide a concepção do sistema em dois grandes modelos que
  se complementam para definir o que o negócio precisa e como isso será
  realizado tecnicamente:
</p>

<ul>
  <li>
    <strong>Modelo Essencial:</strong> Apresenta o sistema em um nível de abstração
    que ignora restrições tecnológicas. O foco é conhecer a essência do negócio e
    o que o sistema deve fazer, independentemente de hardware, software ou se a implementação
    será manual ou automatizada.
  </li>
  <li>
    <strong>Modelo de Implantação:</strong> Define como o sistema será implementado
    em um ambiente técnico específico. Diferente do anterior, este modelo é dependente
    de restrições tecnológicas e considera as características reais do hardware e
    software que serão utilizados.
  </li>
</ul>

<h3>Estrutura do Modelo Essencial</h3>

<p>
  O Modelo Essencial é composto por duas divisões principais, o Modelo Ambiental
  e o Modelo Comportamental, que utilizam ferramentas específicas para detalhar
  o sistema:
</p>

<h4>Modelo Ambiental</h4>

<p>
  Sua função é estabelecer a fronteira entre o sistema e o mundo externo. Ele
  define o escopo por meio de:
</p>

<ul>
  <li>
    <strong>Declaração de Objetivos:</strong> Define a finalidade do sistema.
  </li>
  <li>
    <strong>Diagrama de Contexto:</strong> Representa o sistema como um todo e suas
    interações externas.
  </li>
  <li>
    <strong>Lista de Eventos:</strong> Descreve os estímulos externos que provocam
    uma reação no sistema.
  </li>
</ul>

<h4>Modelo Comportamental</h4>

<p>
  Demonstra as reações internas do sistema aos estímulos recebidos do ambiente.
  Utiliza os métodos de Modelagem de Dados e Modelagem Funcional, representados
  por:
</p>

<ul>
  <li>
    <strong>Diagrama de Fluxo de Dados (DFD) Particionado:</strong> Mostra o funcionamento
    interno das funções.
  </li>
  <li>
    <strong>Modelo Entidade-Relacionamento (MER):</strong> Define a estrutura dos
    dados.
  </li>
  <li>
    <strong>Normalização e Dicionário de Dados:</strong> Organizam e detalham formalmente
    as informações e termos do sistema.
  </li>
</ul>

<h3>Construção dos Diagramas e Modelos</h3>

<p>
  A construção dos modelos na Análise Essencial utiliza representações gráficas
  e textuais para detalhar o funcionamento e a estrutura do sistema. Cada
  ferramenta possui uma finalidade específica dentro dos modelos ambiental e
  comportamental:
</p>

<ul>
  <li>
    <strong>Diagrama de Contexto:</strong> Representa o sistema como uma única "bolha"
    central com seu nome no interior. Ele situa o sistema dentro do negócio, mostrando
    as entidades externas e os fluxos de dados que entram e saem. Entidades repetidas
    são representadas apenas uma vez para manter a clareza.
  </li>
  <li>
    <strong>Lista de Eventos:</strong> É uma relação textual que descreve todos os
    estímulos vindos do ambiente externo que exigem uma resposta ou reação do sistema.
  </li>
  <li>
    <strong>Diagrama de Fluxo de Dados (DFD):</strong> Demonstra como os dados fluem
    e são transformados. Ele conecta processos (nódulos de processamento) onde a
    informação é modificada à medida que percorre o sistema.
  </li>
  <li>
    <strong>Modelo Entidade-Relacionamento (MER):</strong> Oferece uma visão gráfica
    e simplificada da estrutura de dados para o usuário. As entidades são representadas
    por quadros e as linhas de ligação demonstram a lógica dos relacionamentos entre
    elas.
  </li>
  <li>
    <strong>Dicionário de Dados:</strong> Atua como um repositório central de informações.
    Ele fornece descrições textuais detalhadas sobre todos os componentes dos sistemas,
    servindo como um complemento essencial para explicar o que está representado
    nos diagramas.
  </li>
</ul>

<h3>Análise Orientada a Objetos (AOO)</h3>

<p>
  A <strong>Análise Orientada a Objetos</strong> baseia-se na premissa de que o mundo
  real é composto por objetos com propriedades e comportamentos próprios. O objetivo
  dessa abordagem é simular esses elementos no computador, criando componentes que
  organizam dados e funções de forma integrada. A comunicação entre esses componentes
  ocorre por meio de mensagens, definindo como eles interagem e operam dentro do
  sistema.
</p>

<h4>Conceitos Fundamentais</h4>

<p>
  Abaixo estão listados os pilares e termos essenciais para compreender a lógica
  de objetos:
</p>

<ul>
  <li>
    <strong>Objeto:</strong> Representação de conceitos reais (como uma caneta) ou
    abstratos (como uma emoção ou organização) que permitem raciocinar sobre o sistema.
  </li>
  <li>
    <strong>Classe:</strong> Funciona como um molde ou representação técnica de um
    conjunto de objetos, contendo seus atributos e métodos.
  </li>
  <li>
    <strong>Atributos e Métodos:</strong> Atributos são as características que descrevem
    o objeto, enquanto métodos (ou serviços) são as ações e comportamentos que ele
    pode executar.
  </li>
  <li>
    <strong>Abstração:</strong> Princípio que determina a representação apenas das
    características relevantes para o problema, ignorando detalhes desnecessários.
  </li>
  <li>
    <strong>Encapsulamento:</strong> Funciona como uma "caixa-preta", onde os dados
    e os processos internos ficam protegidos e ocultos, sendo acessados apenas por
    interfaces definidas.
  </li>
  <li>
    <strong>Hierarquia de Classes e Herança:</strong> A hierarquia agrupa classes
    em categorias. A herança permite que classes descendentes recebam automaticamente
    atributos e métodos de seus ancestrais, evitando a reescrita de código.
  </li>
  <li>
    <strong>Polimorfismo:</strong> Propriedade que permite que um objeto assuma diferentes
    formas ou responda a uma mesma mensagem de maneiras distintas.
  </li>
  <li>
    <strong>Agregação e Associação:</strong> A agregação permite construir uma classe
    complexa a partir de outras classes componentes. A associação é o mecanismo que
    agrupa objetos que se relacionam em determinado tempo ou circunstância.
  </li>
</ul>

<h4>Perspectiva de Objetos</h4>

<p>
  A essência da metodologia orientada a objetos é analisar o domínio de um
  problema e propor uma solução lógica focada em <strong>objetos</strong>,
  compreendidos como coisas, entidades ou conceitos. Atualmente, a maioria das
  ferramentas de programação suporta essa metodologia, integrando especificação
  e implementação. O uso dessa perspectiva torna os códigos mais compreensíveis
  e aumenta a produtividade, uma vez que facilita a reutilização de recursos já
  desenvolvidos. É um modelo ideal para a construção de sistemas distribuídos e
  aplicações voltadas à internet.
</p>

<h4>Modelos da Metodologia de Objetos</h4>

<p>
  Na descrição de um sistema sob a ótica da orientação a objetos, utilizam-se
  três modelos complementares:
</p>

<ul>
  <li>
    <strong>Modelo de Objetos:</strong> Descreve a estrutura estática do sistema.
    Ele detalha os objetos, seus atributos, operações e os relacionamentos existentes
    entre as classes em um determinado instante.
  </li>
  <li>
    <strong>Modelo Dinâmico:</strong> Apresenta o comportamento do sistema ao longo
    do tempo, focando nas modificações que ocorrem nos objetos e em seus relacionamentos.
  </li>
  <li>
    <strong>Modelo Funcional:</strong> Abrange as funções do sistema, demonstrando
    como os valores de entrada são transformados em valores de saída, independentemente
    da ordem em que o processamento ocorre.
  </li>
</ul>

<h3>Síntese e Revisão Geral</h3>

<p>
  A jornada de aprendizado reforça que o desenvolvimento de sistemas busca,
  acima de tudo, meios claros e analíticos para compreender o que será
  construído. A estruturação lógica permite que funções e componentes sejam
  visualizados de forma organizada antes da implementação técnica.
</p>

<ul>
  <li>
    <strong>Lógica da Orientação a Objetos:</strong> O uso de objetos facilita a
    compreensão das relações entre as partes do sistema. Ao estruturar itens que
    simulam o mundo real, definimos hierarquias, dependências e correlações intuitivas
    para cada componente, tornando o funcionamento do software mais natural e organizado.
  </li>
  <li>
    <strong>Lógica Relacional e Diagramas:</strong> As ferramentas e diagramas estudados
    fornecem a base visual para essa estrutura, permitindo que as conexões entre
    dados e processos sejam mapeadas com precisão.
  </li>
  <li>
    <strong>Foco na Essência:</strong> A Análise Essencial atua como o alicerce desse
    processo, filtrando apenas o que é básico e fundamental para o negócio. Ao deixar
    de lado preocupações tecnológicas momentâneas, o analista garante o entendimento
    do que o sistema "deve ser", assegurando que a solução final atenda ao seu propósito
    real.
  </li>
</ul>
