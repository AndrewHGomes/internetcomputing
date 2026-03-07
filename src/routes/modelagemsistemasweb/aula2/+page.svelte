<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Análise e Modelagem de Sistemas</h2>

<Audios modulo="M8" aulas={["05", "06", "07", "08"]} />

<p>
  A <strong>Análise de Sistemas</strong> é a disciplina fundamental para traduzir
  necessidades de negócio em projetos técnicos. Construir um software é uma atividade
  complexa que exige planejamento estratégico antes da codificação. O objetivo é
  garantir que o sistema não apenas atenda aos requisitos do cliente, mas que o faça
  de forma eficiente, rápida e organizada.
</p>

<p>
  A modelagem de sistemas atua como um estudo dos processos para encontrar o
  melhor caminho lógico para o processamento de informações. Ela utiliza modelos
  para representar a realidade (entidades como alunos ou vendas), as informações
  relacionadas a essas entidades e as funcionalidades que o software deve
  entregar. Essa prática permite visualizar o sistema sob as perspectivas do
  cliente e técnica, validando a viabilidade do projeto.
</p>

<p>
  Com o aumento da dependência global por softwares, a análise de sistemas
  evoluiu para criar métodos que garantam confiabilidade e custo adequado. Três
  grandes métodos de modelagem se destacam nessa evolução: a modelagem
  estruturada, a modelagem essencial e a modelagem orientada a objetos.
</p>

<h4>Objetivos da Modelagem de Sistemas</h4>

<ul>
  <li>Traduzir necessidades de negócio em documentação técnica.</li>
  <li>Planejar o software antes da fase de codificação.</li>
  <li>Representar entidades reais e fluxos de informação.</li>
  <li>Analisar a viabilidade de implementação dos requisitos.</li>
  <li>Definir a solução técnica para o problema apresentado.</li>
</ul>

<h3>Modelagem Estruturada</h3>

<p>
  A <strong>Modelagem Estruturada</strong> fundamenta-se na decomposição de
  problemas complexos em partes menores e mais simples. Seu foco principal
  reside nas <strong>funcionalidades</strong>
  que o software deve entregar para resolver problemas específicos do cliente, como
  a automatização ou simplificação de processos. O objetivo é criar um entendimento
  claro de como cada componente do sistema contribui para a solução global.
</p>

<p>
  Esta metodologia prioriza a construção de um <strong>modelo lógico</strong>,
  focando na inteligência e na regra por trás das funções, em vez de se
  preocupar inicialmente com aspectos físicos ou de hardware. Através de
  técnicas gráficas e visuais, a análise estruturada estabelece uma comunicação
  clara entre usuários, analistas e desenvolvedores, garantindo que todos tenham
  a mesma visão sobre o sistema.
</p>

<p>
  A entrega final deste método é a <strong>especificação do sistema</strong>, um
  documento técnico que traduz a visão do usuário para a linguagem da equipe de
  desenvolvimento. Esta especificação é composta por ferramentas integradas que
  descrevem o comportamento e a estrutura dos dados que circularão no software.
</p>

<h4>Ferramentas da Análise Estruturada</h4>

<ul>
  <li>
    <strong>DFD (Diagrama de Fluxo de Dados):</strong> Representa graficamente o
    caminho dos dados dentro do sistema.
  </li>
  <li>
    <strong>DD (Dicionário de Dados):</strong> Listagem organizada de todos os elementos
    de dados pertinentes ao sistema.
  </li>
  <li>
    <strong>Especificações de Processos:</strong> Descrição detalhada da lógica interna
    de cada funcionalidade mapeada.
  </li>
</ul>

<h3>Diagrama de Fluxo de Dados (DFD)</h3>

<p>
  O <strong>DFD</strong> é a ferramenta central da análise estruturada para mapear
  o caminho dos dados. Como todo software funciona recebendo dados, processando-os
  e transformando-os em informação, o DFD serve para visualizar essa trajetória.
  Ele utiliza uma representação em rede que conecta as funcionalidades do sistema
  aos dados que circulam entre elas.
</p>

<p>
  O foco exclusivo do DFD é <strong>o que</strong> o sistema faz, e não
  <strong>como</strong> ele será implementado. Por ser uma ferramenta de análise
  (e não de projeto), ele busca entender a lógica do fluxo antes de definir tecnologias
  ou métodos de construção. Um DFD bem elaborado deve ser visualmente organizado
  e direto, facilitando a comunicação entre todos os envolvidos no desenvolvimento.
</p>

<p>
  Para lidar com a complexidade, o DFD pode ser organizado em <strong>
    níveis de particionamento
  </strong>. Isso significa que um processo complexo pode ser "quebrado" em
  diagramas menores e mais detalhados, garantindo que o entendimento do todo
  seja construído a partir de partes menores e consistentes entre si.
</p>

<h4>Boas Práticas na Criação de um DFD</h4>

<ul>
  <li>
    <strong>Nomes Significativos:</strong> Utilizar nomenclaturas claras para que
    qualquer pessoa entenda a função de cada componente.
  </li>
  <li>
    <strong>Numeração de Processos:</strong> Identificar cada processo com números
    para facilitar a referência cruzada na documentação.
  </li>
  <li>
    <strong>Estética e Clareza:</strong> Manter o diagrama limpo e organizado para
    evitar confusão visual.
  </li>
  <li>
    <strong>Consistência entre Níveis:</strong> Garantir que o detalhamento de um
    nível inferior respeite as entradas e saídas do nível superior.
  </li>
</ul>

<h4>Componentes do DFD</h4>

<ul>
  <li><strong>Processos:</strong> Representam a transformação dos dados.</li>
  <li><strong>Fluxos de Dados:</strong> Indicam o movimento da informação.</li>
  <li>
    <strong>Depósitos de Dados:</strong> Locais onde os dados são armazenados (como
    arquivos ou bancos de dados).
  </li>
  <li>
    <strong>Entidades:</strong> Origens ou destinos externos dos dados (como usuários
    ou outros sistemas).
  </li>
</ul>

<h3>Componentes do DFD: Detalhamento</h3>

<p>
  O <strong>Diagrama de Fluxo de Dados (DFD)</strong> utiliza quatro componentes
  essenciais para mapear como a informação é transformada e movida dentro de um sistema.
  Cada elemento possui regras específicas de nomenclatura e representação para garantir
  que o modelo seja intuitivo tanto para clientes quanto para técnicos.
</p>

<h4>Processos (Bolhas ou Funções)</h4>

<p>
  O processo é o núcleo do DFD, representando a transformação de dados de
  entrada em dados de saída. Ele altera a estrutura, o conteúdo ou o estado da
  informação. Pode representar tanto tarefas manuais quanto automatizadas.
</p>

<ul>
  <li>
    <strong>Nomenclatura:</strong> Deve usar verbos de ação (ex: Calcular, Emitir,
    Verificar) seguidos pelo objeto (ex: Calcular Média).
  </li>
  <li>
    <strong>Representação:</strong> Geralmente círculos ou retângulos com cantos
    arredondados.
  </li>
</ul>

<h4>Fluxos de Dados</h4>

<p>
  São os caminhos que os dados percorrem entre processos, depósitos e entidades.
  Funcionam como "pacotes" de informação em movimento.
</p>

<ul>
  <li>
    <strong>Nomenclatura:</strong> Substantivos que identifiquem os dados transportados
    (ex: Pedido, Dados do Aluno). Detalhes específicos desses fluxos (como CPF, nome)
    devem ser registrados no Dicionário de Dados (DD).
  </li>
  <li>
    <strong>Representação:</strong> Setas que indicam obrigatoriamente a origem e
    o destino.
  </li>
</ul>

<h4>Depósitos de Dados</h4>

<p>
  Representam dados em repouso, guardados para uso futuro por qualquer
  funcionalidade do sistema. Na fase de análise, não há preocupação com o
  formato técnico (banco de dados ou arquivo físico), apenas com a necessidade
  de armazenamento.
</p>

<ul>
  <li>
    <strong>Nomenclatura:</strong> Deve-se usar o <strong>plural</strong> para indicar
    uma coleção de registros (ex: Clientes, Produtos, Vendas).
  </li>
  <li>
    <strong>Representação:</strong> Duas linhas paralelas ou um retângulo aberto
    lateralmente.
  </li>
</ul>

<h4>Entidades (Terminadores)</h4>

<p>
  São os pontos externos que dão origem aos dados ou os recebem do sistema.
  Podem ser pessoas, departamentos ou até mesmo outros sistemas integrados.
</p>

<ul>
  <li>
    <strong>Nomenclatura:</strong> Utiliza-se o
    <strong>plural e letras maiúsculas</strong> para distinção (ex: CLIENTES, FORNECEDORES).
    Se for um software externo, inclui-se a palavra "Sistema" (ex: SISTEMA CONTÁBIL).
  </li>
  <li><strong>Representação:</strong> Retângulos.</li>
</ul>

<h4>Boas Práticas de Nomenclatura</h4>

<ul>
  <li>
    <strong>Processos:</strong> Verbo no infinitivo + Objeto (Gerar Relatório).
  </li>
  <li><strong>Fluxos:</strong> Nome do conjunto de dados (Nota Fiscal).</li>
  <li><strong>Depósitos:</strong> Substantivo no plural (Estoques).</li>
  <li>
    <strong>Entidades:</strong> Substantivo no plural e MAIÚSCULO (USUÁRIOS).
  </li>
</ul>

<h3>Organização de um DFD em Níveis</h3>

<p>
  O <strong>DFD</strong> deve ser organizado em níveis para evitar que a
  complexidade do sistema torne o diagrama confuso. Essa técnica, chamada de
  <strong>particionamento</strong>, permite que o analista apresente o
  funcionamento do software de forma progressiva: do nível mais macro (visão
  geral) até o nível mais detalhado (visão específica).
</p>

<p>
  O limite para a criação desses níveis é a clareza. Enquanto houver processos
  complexos que precisem de mais explicações para serem desenvolvidos, novos
  subníveis devem ser criados. O objetivo é que cada diagrama seja simples o
  suficiente para ser lido e mantido sem ambiguidades.
</p>

<h4>Níveis Hierárquicos do DFD</h4>

<ul>
  <li>
    <strong>DFD de Contexto (Nível Superior):</strong> Representa o sistema como
    um único processo central. Mostra apenas as entidades externas (quem interage
    com o sistema) e os fluxos principais de entrada e saída. Não detalha processos
    internos nem depósitos de dados.
  </li>
  <li>
    <strong>DFD de Nível Zero (Diagrama de Visão Geral):</strong> Expande o processo
    único do contexto, revelando as principais funcionalidades (processos) do software.
    Aqui já aparecem os primeiros depósitos de dados e a divisão entre as grandes
    áreas do sistema.
  </li>
  <li>
    <strong>DFDs de Níveis Intermediários (Nível 1, 2, etc.):</strong> São as decomposições
    dos processos do nível zero. Se um processo de "Vendas" é complexo, ele é quebrado
    em um novo diagrama que detalha as etapas internas dessa venda.
  </li>
</ul>

<h4>Benefícios da Organização em Níveis</h4>

<ul>
  <li>
    <strong>Comunicação:</strong> Facilita o entendimento de usuários (níveis altos)
    e desenvolvedores (níveis baixos).
  </li>
  <li>
    <strong>Manutenção:</strong> É mais fácil corrigir ou alterar uma parte específica
    do sistema sem afetar a visão do todo.
  </li>
  <li>
    <strong>Consistência:</strong> Garante que os dados que entram em um nível macro
    sejam os mesmos processados nos níveis detalhados.
  </li>
</ul>

<h3>Conclusão: Análise Estruturada e o Valor do DFD</h3>

<p>
  Nesta etapa final, o foco recai sobre a <strong>Análise Estruturada</strong> e
  sua principal ferramenta, o <strong>DFD (Diagrama de Fluxo de Dados)</strong>.
  A modelagem lógica de sistemas busca descrever o comportamento do software sem
  se prender a detalhes técnicos de implementação, garantindo que a solução
  proposta esteja alinhada às expectativas do cliente.
</p>

<p>
  O DFD destaca-se como uma ferramenta de comunicação poderosa entre a equipe
  técnica e os usuários. Por ser um modelo visual e conceitualmente simples, ele
  permite que o cliente valide o fluxo de informações e identifique falhas ou
  omissões nos requisitos logo no início do projeto, evitando retrabalho custoso
  nas fases de codificação e testes.
</p>

<p>
  A modelagem de sistemas transforma a complexidade do desenvolvimento em
  modelos visuais claros, definidos e diretos. O uso dessas técnicas é o que
  garante que o software final seja uma solução robusta para o problema
  original, mantendo o foco no processamento eficiente dos dados.
</p>

<h4>Benefícios Centrais da Abordagem</h4>

<ul>
  <li>
    <strong>Identificação Precoce de Falhas:</strong> Permite corrigir erros de lógica
    antes do início da programação.
  </li>
  <li>
    <strong>Validação com o Usuário:</strong> Facilita a confirmação de que os dados
    e processos modelados atendem ao negócio.
  </li>
  <li>
    <strong>Simplicidade Visual:</strong> Reduz a complexidade por meio de representações
    gráficas intuitivas.
  </li>
  <li>
    <strong>Foco no Dado:</strong> Garante que todas as informações necessárias para
    as funcionalidades estejam mapeadas.
  </li>
</ul>
