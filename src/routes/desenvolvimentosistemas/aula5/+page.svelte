<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Engenharia de Software: Conceitos e Fundamentos</h2>

<Audios modulo="M10" aulas={["17", "18", "19", "20"]} />

<p>
  A <strong>Engenharia de Software</strong> consiste na aplicação de métodos científicos
  e técnicas sistemáticas para o desenvolvimento de sistemas. Diferente da codificação
  isolada, ela organiza o processo por meio de teorias, modelos e ferramentas da
  ciência da computação para garantir a utilização eficiente de recursos. Seu objetivo
  principal é promover as melhores práticas, integrando o desenvolvimento técnico
  ao gerenciamento de projetos e à documentação formal.
</p>

<p>
  O desenvolvimento eficaz exige que o profissional compreenda não apenas as
  linguagens de programação, mas também o <strong>universo de negócios</strong> do
  cliente. Essa visão ampla permite estruturar melhor os componentes do sistema e
  aumentar a efetividade da solução proposta.
</p>

<h4>Características do Software</h4>

<p>
  Diferente de produtos físicos, o software possui propriedades abstratas que
  moldam como ele deve ser gerenciado:
</p>

<ul>
  <li>
    <strong>Invisibilidade:</strong> O software não possui presença física tangível.
  </li>
  <li>
    <strong>Complexidade:</strong> Apresenta múltiplas conexões e interdependências
    lógicas.
  </li>
  <li>
    <strong>Mutabilidade:</strong> Necessita de atualizações constantes para acompanhar
    as mudanças do mundo.
  </li>
  <li>
    <strong>Conformidade:</strong> O software deve ser adaptado para operar conforme
    as regras e restrições do ambiente em que está inserido.
  </li>
</ul>

<h4>Estrutura da Engenharia de Software</h4>

<p>A disciplina se sustenta em três pilares que conectam a teoria à prática:</p>

<ul>
  <li>
    <strong>Métodos:</strong> Detalham como construir o sistema, abrangendo desde
    o planejamento e análise de requisitos até a codificação, testes e manutenção.
  </li>
  <li>
    <strong>Ferramentas:</strong> Promovem a automação dos métodos, exemplificadas
    pelas ferramentas CASE (Computer-Aided Software Engineering).
  </li>
  <li>
    <strong>Procedimentos:</strong> Estabelecem a ponte entre métodos e ferramentas,
    definindo sequências de aplicação, entregas (produtos), formas de controle e
    marcos de referência.
  </li>
</ul>

<h4>Ciclo de Vida do Software</h4>

<p>
  O processo de criação e evolução de um sistema é dividido em quatro fases
  principais:
</p>

<ol>
  <li>
    <strong>Definição:</strong> Fase preliminar de análise de viabilidade, levantamento
    de requisitos, estimativas de prazos e custos, identificação de riscos e formalização
    de contratos.
  </li>
  <li>
    <strong>Desenvolvimento:</strong> Envolve o design (arquitetura, interface e
    algoritmos), a implementação (codificação e integração) e a validação (testes
    de desempenho, usabilidade e correção de erros).
  </li>
  <li>
    <strong>Operação:</strong> Fase de instalação, configuração e uso real pelo cliente.
    Inclui o suporte operacional, correção de falhas em ambiente de produção e o
    lançamento de novas versões.
  </li>
  <li>
    <strong>Retirada:</strong> Envolve o encerramento do ciclo do produto, processos
    de migração de dados e atividades de reengenharia para modernização ou substituição
    do sistema.
  </li>
</ol>

<h3>Engenharia de Requisitos</h3>

<p>
  A <strong>Engenharia de Requisitos</strong> foca na definição e manutenção de documentos
  que descrevem o que o sistema deve fazer e sob quais restrições ele deve operar.
  O processo busca transformar necessidades vagas dos usuários em especificações
  técnicas precisas para guiar o desenvolvimento. O fluxo de trabalho da Engenharia
  de Requisitos baseia-se em quatro etapas principais:
</p>

<ul>
  <li>
    <strong>Estudo de Viabilidade:</strong> Avalia se o projeto vale a pena ser executado.
    Analisa a relação entre o esforço de desenvolvimento e os benefícios esperados,
    identificando problemas, inconsistências e riscos antes da tomada de decisão
    sobre a continuidade do software.
  </li>
  <li>
    <strong>Descoberta e Análise:</strong> Momento de entender as necessidades dos
    usuários, os objetivos a serem atingidos e as funções que o sistema precisa desempenhar.
  </li>
  <li>
    <strong>Especificação:</strong> Tradução das necessidades em um documento formal
    que descreve detalhadamente as demandas do usuário e do sistema.
  </li>
  <li>
    <strong>Validação:</strong> Verificação técnica para garantir que os requisitos
    definidos realmente atendem às necessidades do negócio e que estão descritos
    de forma clara e correta.
  </li>
</ul>

<h4>Classificação dos Requisitos</h4>

<p>
  Os requisitos são divididos em duas categorias fundamentais para a
  estruturação do sistema:
</p>

<ul>
  <li>
    <strong>Requisitos Funcionais:</strong> Descrevem as funções e ações que o sistema
    deve executar. Representam o "o que" o software faz (ex: gerar um relatório,
    realizar um cadastro).
  </li>
  <li>
    <strong>Requisitos Não Funcionais:</strong> Definem características, restrições
    e propriedades de qualidade do sistema. Referem-se ao "como" o sistema deve se
    comportar (ex: usabilidade, segurança, desempenho, confiabilidade e portabilidade).
  </li>
</ul>

<h4>Importância da Documentação</h4>

<p>
  Todo o processo de análise deve ser documentado para servir de guia durante o
  desenvolvimento e permitir melhorias futuras. Essa estrutura organizada
  garante que o produto final seja viável e entregue os resultados esperados
  pelos interessados.
</p>

<h3>Gerenciamento de Requisitos</h3>

<p>
  O <strong>Gerenciamento de Requisitos</strong> consiste no processo de compreender,
  planejar, monitorar e controlar as necessidades de um sistema ao longo de todo
  o seu ciclo de vida. Ele atua como uma etapa investigativa que transforma informações
  em um plano de ação, garantindo que os objetivos propostos sejam atingidos e que
  as funções e restrições do software sejam respeitadas. Este processo estruturado
  permite realizar a análise de viabilidade e fornece os subsídios necessários para
  a tomada de decisão estratégica no projeto de desenvolvimento.
</p>

<h4>Aspectos Fundamentais da Gerência</h4>

<p>
  Para que a gestão seja eficiente, não basta apenas listar desejos; é preciso
  aplicar mecanismos de controle e qualidade:
</p>

<ul>
  <li>
    <strong>Rastreamento:</strong> Identifica as dependências entre os requisitos,
    suas origens e como eles se associam ao projeto final. Divide-se em rastreamento
    de origem (propostas iniciais), associação entre requisitos dependentes e associação
    entre requisitos e o projeto.
  </li>
  <li>
    <strong>Controle de Mudanças:</strong> Estabelece processos para gerenciar alterações
    decorrentes de novas tecnologias, mudanças no ambiente de negócio ou falhas na
    definição inicial. Toda mudança deve ser documentada e avaliada antes da implementação.
  </li>
  <li>
    <strong>Gerência de Configuração:</strong> Divide-se em
    <strong>controle de versões</strong>
    (gestão das diferentes iterações de um item) e
    <strong>controle de configuração</strong> (manutenção do conjunto de artefatos
    que formam uma configuração específica do sistema).
  </li>
  <li>
    <strong>Garantia de Qualidade:</strong> Assegura que os requisitos foram especificados
    corretamente no papel e que, ao final do processo, a execução técnica entrega
    exatamente o que foi validado.
  </li>
</ul>

<h4>Planejamento e Execução</h4>

<p>
  O planejamento de requisitos utiliza os métodos da Engenharia de Requisitos
  para compreender a natureza dos problemas e definir as funções que o sistema
  deve desempenhar. Ele organiza as possibilidades e restrições, servindo como o
  norteador que alinha a execução técnica às expectativas dos interessados.
</p>

<h3>Refinamento de Requisitos</h3>

<p>
  O <strong>Refinamento</strong> é o processo de "apurar" os requisitos, realizando
  uma revisão detalhada para torná-los mais claros, precisos e adequados ao projeto.
  O objetivo é eliminar ambiguidades e garantir que a equipe de desenvolvimento compreenda
  exatamente o que deve ser construído, evitando retrabalho e falhas na entrega.
</p>

<p>
  Este processo envolve a identificação de lacunas, elementos faltantes e a
  verificação da consistência de cada item listado. Quando um problema é
  detectado, deve haver uma negociação com os envolvidos (stakeholders) para
  ajustar as expectativas e garantir a viabilidade da execução.
</p>

<h4>Problemas Comuns no Refinamento</h4>

<p>
  Durante a revisão, o analista busca identificar e corrigir falhas estruturais
  nos requisitos, tais como:
</p>

<ul>
  <li>
    <strong>Ambiguidade:</strong> Requisitos com falta de clareza que permitem múltiplas
    interpretações.
  </li>
  <li>
    <strong>Parcialidade:</strong> Requisitos incompletos que não fornecem todas
    as informações necessárias para a implementação.
  </li>
  <li>
    <strong>Requisitos Múltiplos:</strong> Quando vários requisitos são agrupados
    em um único texto, dificultando a gestão e o teste; estes devem ser separados.
  </li>
  <li>
    <strong>Requisitos com Alternativas:</strong> Descrições que não definem uma
    ação clara, deixando margem para dúvidas sobre qual caminho o sistema deve seguir.
  </li>
</ul>

<h4>Critérios de um Requisito Refinado</h4>

<p>
  Para que um requisito seja considerado pronto para a próxima fase, ele deve
  ser:
</p>

<ul>
  <li><strong>Claro e bem definido:</strong> Sem margem para dúvidas.</li>
  <li>
    <strong>Consistente:</strong> Não deve contradizer outros requisitos do sistema.
  </li>
  <li>
    <strong>Verificável:</strong> Deve ser possível testar e comprovar que o requisito
    foi atendido após o desenvolvimento.
  </li>
</ul>

<p>
  Ao garantir que os requisitos possuam essas qualidades, o refinamento
  estabelece a base necessária para a <strong>Validação</strong> e a criação da
  <strong>Matriz de Rastreabilidade</strong>.
</p>

<h3>Validação de Requisitos e Matriz de Rastreabilidade</h3>

<p>
  A <strong>Validação de Requisitos</strong> foca na análise do conjunto completo
  de requisitos para garantir que eles correspondam exatamente às necessidades do
  cliente. Enquanto o refinamento analisa cada item isoladamente para verificar clareza
  e completude, a validação observa o todo para identificar conflitos, falhas de
  especificação e inconsistências antes do início do desenvolvimento.
</p>

<p>
  Validar é essencial para evitar custos elevados. Em sistemas de grande porte,
  corrigir erros de requisitos após o software já estar em uso é muito mais caro
  do que identificá-los na fase de planejamento. O processo exige a participação
  ativa do cliente para confirmar a documentação e reduzir questionamentos
  futuros. As principais técnicas de validação incluem:
</p>

<ul>
  <li>
    <strong>Verificação de Validade:</strong> Revisão manual e técnica dos requisitos.
  </li>
  <li>
    <strong>Prototipação:</strong> Criação de modelos visuais para validar a interpretação
    das funções.
  </li>
  <li>
    <strong>Geração de Casos de Teste:</strong> Definição de como cada requisito
    será testado.
  </li>
  <li>
    <strong>Consistência Automática:</strong> Uso de ferramentas para cruzar dados
    e encontrar contradições.
  </li>
</ul>

<h4>Matriz de Rastreabilidade</h4>

<p>
  A <strong>Matriz de Rastreabilidade</strong> é a ferramenta que mapeia as relações
  entre os requisitos e os demais componentes do sistema. Sua função principal é
  servir de base para a definição do escopo e permitir a análise de impacto: se um
  requisito mudar, a matriz mostra exatamente quais outros pontos do projeto serão
  afetados. Os principais tipos de rastreabilidade são:
</p>

<ul>
  <li>
    <strong>Funcionalidades:</strong> Conexão entre o que foi pedido e o que será
    entregue.
  </li>
  <li>
    <strong>Fontes:</strong> Identificação de quem (ou de onde) surgiu a demanda
    do requisito.
  </li>
  <li>
    <strong>Subsistemas:</strong> Relação entre os requisitos e as partes específicas
    do software.
  </li>
  <li>
    <strong>Interfaces:</strong> Mapeamento de como os requisitos interagem com outros
    sistemas ou usuários.
  </li>
</ul>

<p>
  Essa matriz geralmente utiliza um formato de cruzamento de dados, permitindo
  localizar rapidamente pontos de intersecção e dependência, garantindo maior
  controle sobre a evolução do software.
</p>

<h3>Conclusão: O Valor da Engenharia de Software</h3>

<p>
  O encerramento deste conteúdo reforça que, embora o conceito de <strong>
    Engenharia de Software
  </strong> seja simples; a aplicação de métodos para organizar o desenvolvimento,
  sua execução exige rigor, critério e atenção aos detalhes. O uso de métodos científicos
  permite compreender o sistema antes da codificação, o que reduz substancialmente
  o risco de falhas e o desperdício de recursos.
</p>

<h4>Síntese do Processo de Requisitos</h4>

<p>
  Os requisitos são o pilar central para garantir que o sistema final seja
  lógico e integrado. O sucesso do projeto depende de um fluxo bem executado:
</p>

<ul>
  <li>
    <strong>Identificação e Gerenciamento:</strong> Capturar as necessidades e planejar
    como serão atendidas.
  </li>
  <li>
    <strong>Refinamento:</strong> Eliminar ambiguidades e detalhar cada funcionalidade.
  </li>
  <li>
    <strong>Validação:</strong> Garantir que o conjunto de requisitos atende ao que
    o cliente realmente precisa.
  </li>
  <li>
    <strong>Rastreabilidade:</strong> Mapear as conexões entre requisitos para entender
    os impactos de qualquer mudança.
  </li>
</ul>

<p>
  A Engenharia de Software, portanto, transforma o desenvolvimento de sistemas
  em um processo previsível, focado na entrega de valor e na qualidade técnica.
</p>
