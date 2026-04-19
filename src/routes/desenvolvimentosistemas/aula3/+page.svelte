<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Análise Estruturada</h2>

<Audios modulo="M12" aulas={["09", "10", "11", "12"]} />

<p>
  O desenvolvimento de sistemas exige condições técnicas específicas para
  garantir que o produto final atenda às necessidades do cliente. A estruturação
  do trabalho envolve o estudo do <strong>Ciclo de Vida do Software</strong>, da
  <strong>Análise Estruturada</strong> (incluindo DFD), da
  <strong>Especificação de Processos</strong> e do
  <strong>Dicionário de Dados</strong>. Essas ferramentas permitem visualizar o
  fluxo de informações, compreender a codificação e organizar os dados do
  projeto.
</p>

<h3>Ciclo de Vida de Software</h3>

<p>
  Ciclo de Vida de Software O ciclo de vida compreende todas as etapas de um
  software, desde a concepção da ideia inicial até a sua descontinuação. A
  definição dessas etapas é crucial para o planejamento, controle de processos,
  cumprimento de prazos e garantia de resultados. A falta de um ciclo bem
  definido geralmente resulta em atrasos, custos elevados e entregas que não
  condizem com a expectativa do usuário.
</p>

<p>
  Para um desenvolvimento eficiente, o profissional não deve dominar apenas
  linguagens de programação, mas também entender profundamente o contexto e a
  área de negócio onde o software será aplicado (como a área médica ou
  financeira). O desenvolvedor deve analisar os processos junto aos solicitantes
  para identificar as melhores práticas e garantir que a ferramenta facilite as
  atividades cotidianas.
</p>

<h4>Principais Modelos de Ciclo de Vida:</h4>

<p>
  Os modelos de ciclo de vida organizam o fluxo de trabalho de formas distintas,
  variando entre abordagens rígidas e metodologias ágeis. A escolha do modelo
  ideal depende da experiência da equipe, da complexidade do sistema e da
  clareza dos requisitos iniciais.
</p>

<ul>
  <li>
    <strong>Cascata (Waterfall):</strong> Modelo tradicional e rígido, onde uma fase
    só começa quando a anterior termina. Segue a ordem: Requisitos &rarr; Planejamento
    &rarr; Implementação &rarr; Testes &rarr; Integração. É fácil de entender, mas
    difícil de adaptar a mudanças.
  </li>
  <li>
    <strong>Prototipagem:</strong> Foca na construção de versões preliminares (protótipos)
    para ajudar o cliente a visualizar e validar requisitos, especialmente quando
    eles não estão claros desde o início.
  </li>
  <li>
    <strong>Modelos Iterativos e Ágeis (Incremental, Espiral, RAD):</strong> Permitem
    que o planejamento e o desenvolvimento ocorram em ciclos menores, facilitando
    correções rápidas e maior velocidade de entrega.
  </li>
  <li>
    <strong>RUP (Rational Unified Process):</strong> Um framework que utiliza as
    melhores práticas de engenharia, organizando o desenvolvimento em fases com foco
    na redução de riscos e arquitetura sólida.
  </li>
</ul>

<h3>Análise Estruturada</h3>

<p>
  A análise estruturada é uma metodologia que utiliza <strong
    >modelos gráficos</strong
  > para produzir uma especificação funcional do sistema. Ela define as funções e
  as estruturas de dados de forma visual, facilitando a comunicação e o entendimento
  comum entre desenvolvedores e usuários. O objetivo principal é aplicar técnicas
  que organizem a compreensão do sistema, buscando sempre as melhores práticas de
  implementação.
</p>

<h4>Modelo Ambiental</h4>

<p>
  Este modelo descreve como o sistema interage com o meio externo e responde às
  demandas do contexto onde será utilizado. Ele foca nos limites do software e
  em sua finalidade.
</p>

<ul>
  <li>
    <strong>Definição de objetivos:</strong> Estabelece a finalidade principal do
    sistema.
  </li>
  <li>
    <strong>Lista de eventos:</strong> Relação de acontecimentos externos que provocam
    uma reação ou interação com o sistema.
  </li>
  <li>
    <strong>Diagrama de contexto:</strong> Representação gráfica que mostra o sistema
    como um processo único e suas conexões com entidades externas.
  </li>
</ul>

<h4>Modelo Comportamental</h4>

<p>
  O modelo comportamental detalha as ações internas que o sistema deve realizar
  para processar os dados e responder aos eventos definidos no modelo ambiental.
  Ele utiliza técnicas específicas para mapear o comportamento lógico do
  software:
</p>

<ul>
  <li>
    <strong>Diagrama de Fluxo de Dados (DFD):</strong> Demonstra o caminho e a transformação
    dos dados.
  </li>
  <li>
    <strong>Dicionário de Dados (DD):</strong> Catalogação detalhada de todos os
    elementos de dados.
  </li>
  <li>
    <strong>Diagrama de Entidade e Relacionamento (DER):</strong> Modelagem da estrutura
    de dados e suas ligações.
  </li>
  <li>
    <strong>Especificação de Processos (EP):</strong> Descrição detalhada da lógica
    de cada processo.
  </li>
  <li>
    <strong>Diagrama de Transição de Estados (DTE):</strong> Mostra como o sistema
    muda de um estado para outro conforme ocorrem eventos.
  </li>
</ul>

<h3>Ferramentas de Visualização (Diagramas)</h3>

<p>
  A estrutura da análise é consolidada através de diversos diagramas e tabelas
  que garantem clareza e lógica ao desenvolvimento. Além dos já citados
  (Contexto, DFD, DER, DTE), utilizam-se listas de eventos, tabelas de decisão e
  árvores de decisão para mapear fluxos complexos e garantir que o produto final
  seja compreensível para todos os envolvidos no projeto.
</p>

<h4>Diagrama de Fluxo de Dados (DFD)</h4>

<p>
  O DFD é uma representação gráfica de uma rede de processos interligados,
  funcionando como um modelo intuitivo que facilita a comunicação entre
  desenvolvedores e usuários. Sua estrutura segue a lógica <strong
    >top-down</strong
  >, organizando-se em níveis hierárquicos que partem de uma visão geral para o
  detalhamento progressivo. Por ser um modelo interativo, ele permite
  refinamentos constantes conforme as discussões entre os envolvidos avançam.
</p>

<p>
  Diferente de um fluxograma, o DFD <strong>não é procedimental</strong>. Isso
  significa que ele foca exclusivamente no fluxo de informações e não no fluxo
  de controle. Ele não demonstra ciclos, processamentos condicionais (como "se"
  ou "então"), sequências temporais ou cronogramas, limitando-se a mostrar como
  o dado caminha e se transforma dentro do sistema.
</p>

<h4>Componentes e Regras de Construção</h4>

<p>
  A construção de um DFD exige a observação de regras estritas sobre como os
  dados circulam entre os elementos do sistema. Os principais componentes são:
</p>

<ul>
  <li>
    <strong>Depósito de Dados:</strong> Representa onde as informações são
    armazenadas (ex: Clientes, Pedidos). Os dados nunca podem se mover
    diretamente entre dois depósitos ou entre um depósito e uma entidade
    externa; eles devem sempre passar por um <strong>processo</strong> intermediário.
  </li>
  <li>
    <strong>Entidades Externas:</strong> Representam a origem ou o destino dos dados
    fora do sistema (ex: Fornecedores, Cliente). Não é permitido o fluxo direto entre
    duas entidades externas dentro do DFD, pois o diagrama foca apenas no que é de
    interesse para o processamento do sistema.
  </li>
  <li>
    <strong>Fluxo de Dados:</strong> Representado por setas rotuladas, indica a rota
    e o deslocamento da informação entre processos, entidades e depósitos. Serve
    como a interface entre os componentes, detalhando as entradas e saídas.
  </li>
</ul>

<h4>Simbologia e Utilidade</h4>

<p>
  O DFD utiliza símbolos padronizados como retângulos, círculos (ou retângulos
  arredondados para processos) e flechas. Os rótulos devem ser curtos e
  objetivos para garantir a clareza. Sua grande vantagem é traduzir visualmente
  elementos técnicos complexos, tornando a lógica de manuseio de dados
  compreensível para o cliente e precisa para a equipe técnica, podendo ser
  elaborado desde esboços manuais rápidos até diagramas altamente detalhados.
</p>

<h3>Especificação de Processos</h3>

<p>
  A especificação de processos tem como objetivo descrever a lógica de
  transformação dos dados de entrada em dados de saída. Enquanto o DFD mostra o
  caminho dos dados, a especificação detalha o que acontece dentro de cada
  processo. Essa descrição pode ser feita utilizando linguagem natural
  estruturada ou pseudocódigos.
</p>

<h4>Formas de Especificação</h4>

<ul>
  <li>
    <strong>Português Estruturado:</strong> Utiliza o idioma nativo de forma técnica
    para descrever a função. Deve-se priorizar verbos no imperativo e termos padronizados
    do dicionário de dados. É fundamental evitar adjetivos ou advérbios, focando
    em construções de lógica de programação como sequências, decisões e repetições.
  </li>
  <li>
    <strong>Pseudocódigos:</strong> São descrições orientadas à implementação que
    se assemelham a uma linguagem de programação, mas sem a rigidez sintática total
    de um compilador. Sua função é facilitar a tradução da lógica para a codificação
    definitiva.
  </li>
</ul>

<h4>Diretrizes de Escrita</h4>

<p>
  Para que a especificação seja eficiente, ela deve seguir os princípios da
  programação estruturada. A clareza na escrita garante que o desenvolvedor
  compreenda exatamente quais regras de negócio devem ser aplicadas, servindo
  como uma ponte entre o modelo gráfico e a escrita do código-fonte final.
</p>

<h3>Dicionário de Dados</h3>

<p>
  O Dicionário de Dados funciona como uma tabela de referência que define e
  padroniza todos os elementos de dados utilizados no desenvolvimento do
  sistema. Assim como um dicionário convencional, sua finalidade é servir como
  fonte de consulta para garantir que desenvolvedores e usuários tenham a mesma
  compreensão sobre o significado e a representação de cada informação.
</p>

<h4>Conteúdo e Estrutura</h4>

<p>
  Embora não exista uma obrigatoriedade de incluir todos os campos, quanto mais
  detalhado for o dicionário, mais eficiente será o suporte ao desenvolvimento e
  às futuras manutenções do software. As informações mais comuns encontradas
  são:
</p>

<ul>
  <li>
    <strong>Identificação:</strong> Nome principal do item e seus Aliases (outros
    nomes pelos quais o dado é conhecido).
  </li>
  <li>
    <strong>Contexto de Uso:</strong> Listagem de onde e como o dado é utilizado
    nos processos.
  </li>
  <li>
    <strong>Definições Técnicas:</strong> Descrição detalhada do conteúdo, definição
    precisa dos elementos e descrição de objetos.
  </li>
  <li>
    <strong>Regras e Restrições:</strong> Restrições de integridade, perfis de usuários,
    papéis e privilégios de acesso.
  </li>
  <li>
    <strong>Dados de Implementação:</strong> Alocações de espaço em memória/disco,
    índices e informações de verificação.
  </li>
  <li>
    <strong>Notas Complementares:</strong> Observações adicionais que auxiliem na
    compreensão do dado.
  </li>
</ul>

<h4>Importância no Projeto</h4>

<p>
  O uso do dicionário de dados elimina ambiguidades e evita que diferentes
  membros da equipe interpretem o mesmo dado de formas distintas. Ele atua como
  o "repositório central de definições", sendo indispensável para manter a
  consistência entre o Diagrama de Fluxo de Dados (DFD), a Especificação de
  Processos e o banco de dados final.
</p>

<h3>Conclusão e Integração de Conceitos</h3>

<p>
  A análise estruturada e seus componentes formam um conjunto integrado que
  amplia a visão de técnicos e clientes sobre o sistema. A eficiência de um
  software não reside apenas na codificação, mas na capacidade de o
  desenvolvedor compreender e modelar a <strong
    >dinâmica dos processos organizacionais</strong
  >, garantindo que a tecnologia seja efetiva para o negócio.
</p>

<h4>A Conexão entre os Temas</h4>

<p>
  Os conceitos estudados não são isolados, mas dependentes entre si para formar
  uma estrutura lógica de desenvolvimento:
</p>

<ul>
  <li>
    <strong>Ciclo de Vida:</strong> Fornece a estrutura temporal e as fases (o contexto
    conhecido).
  </li>
  <li>
    <strong>Modelagem (DFD):</strong> Oferece a visão gráfica dos processos dentro
    de cada fase do ciclo.
  </li>
  <li>
    <strong>Especificação de Processos:</strong> Detalha a lógica interna de cada
    item do fluxo.
  </li>
  <li>
    <strong>Dicionário de Dados:</strong> Padroniza a linguagem e os elementos usados
    em todos os modelos anteriores.
  </li>
</ul>

<p>
  A união dessas ferramentas permite que o desenvolvimento ocorra de forma
  organizada, com padrões claros que facilitam tanto a criação inicial quanto as
  manutenções futuras, sempre focando em transformar a realidade da organização
  em um sistema funcional e lógico.
</p>
