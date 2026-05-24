<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Normas e o Profissional de Segurança Digital</h2>

<Audios modulo="M16" aulas={["09", "10", "11", "12"]} />

<p>
  As normas de segurança não são exclusivas da engenharia tradicional; elas são
  fundamentais para estabelecer padrões mínimos e referências básicas na
  construção de sistemas digitais seguros. No desenvolvimento de aplicações, o
  conhecimento das ameaças deve ser aliado às recomendações normativas desde a
  elaboração do código, garantindo que a segurança seja nativa e não apenas um
  ajuste posterior.
</p>

<p>
  O profissional de TI, independentemente de ser um especialista em segurança,
  deve manter-se atualizado sobre essas publicações internacionais. Isso ocorre
  porque todos os aplicativos estão expostos a riscos, e as normas oferecem as
  diretrizes necessárias para adotar medidas preventivas eficazes em qualquer
  projeto tecnológico.
</p>

<h4>Categorias de Atuação do Profissional de Segurança (NIST)</h4>

<p>
  De acordo com o National Institute of Standards and Technology (NIST), o
  especialista em segurança cibernética atua em frentes distintas para garantir
  a integridade dos dados:
</p>

<ul>
  <li>
    <strong>Operar e manter:</strong> suporte, administração e manutenção para assegurar
    desempenho e segurança dos sistemas.
  </li>
  <li>
    <strong>Proteger e defender:</strong> identificação, análise e mitigação de ameaças
    às redes e sistemas internos.
  </li>
  <li>
    <strong>Investigar:</strong> análise e detecção de incidentes ou crimes digitais
    que utilizam recursos de TI.
  </li>
  <li>
    <strong>Coletar e operar:</strong> coleta de dados de inteligência cibernética
    e atuação contra operações de negação de serviço e fraudes.
  </li>
</ul>

<p>
  Para desempenhar essas funções, o profissional exige um vasto conhecimento
  técnico e uma atualização constante, dado que o cenário de ameaças digitais
  evolui rapidamente.
</p>

<h3>Normas e Certificações em Segurança</h3>

<p>
  A busca por atualização em Segurança da Informação exige o uso de <strong>
    fontes confiáveis
  </strong> para evitar informações conflitantes. A adoção de normas técnicas garante
  que um sistema atenda aos requisitos mínimos de segurança estabelecidos por especialistas
  internacionais, servindo como um guia padronizado para o desenvolvimento e gestão
  de dados.
</p>

<h4>Instituições e Normas Principais</h4>

<p>No Brasil e no mundo, órgãos específicos regulamentam esses padrões:</p>

<ul>
  <li>
    <strong>ABNT (Associação Brasileira de Normas Técnicas):</strong>
    Responsável pela publicação de normas no Brasil. A família de normas NBR
    <strong>ISO/IEC 27000</strong> é a principal referência para a Gestão da Segurança
    da Informação.
  </li>
  <li>
    <strong>ISO/IEC:</strong> Cooperação internacional (International Organization
    for Standardization e International Electrotechnical Commission) que define padrões
    globais, como a ISO 9000 (qualidade) e a ISO 27000 (segurança).
  </li>
</ul>

<h4>Certificações Profissionais</h4>

<p>
  As certificações são selos de competência que validam o conhecimento de um
  profissional perante o mercado. Elas funcionam como um filtro para empresas,
  substituindo testes técnicos complexos no ato da contratação.
</p>

<ul>
  <li>
    <strong>ISO 27000:</strong> Certifica profissionais na implementação de Sistemas
    de Gestão de Segurança da Informação.
  </li>
  <li>
    <strong>CISSP (Certified Information Systems Security Professional):</strong
    >
    Uma das certificações mais reconhecidas mundialmente, promovida pela instituição
    <strong>ISC2</strong>.
  </li>
  <li>
    <strong>Processo de Obtenção:</strong> Para ser certificado, o profissional deve
    ser aprovado em um exame rigoroso que comprova seu domínio sobre o conteúdo indicado
    pelas instituições certificadoras.
  </li>
</ul>

<h3>Legislação e a LGPD</h3>

<p>
  A segurança digital não depende apenas de tecnologia, mas também de um amparo
  jurídico que garanta a privacidade e a proteção das informações. No Brasil, a
  principal referência é a <strong>Lei Geral de Proteção de Dados (LGPD)</strong
  >, ou Lei nº 13.709/2018, que estabelece regras sobre como empresas e órgãos
  públicos devem coletar, armazenar e compartilhar dados pessoais.
</p>

<h4>Pontos Chave da LGPD</h4>

<p>
  A lei visa criar um cenário de segurança jurídica tanto no meio digital quanto
  no físico, protegendo o cidadão brasileiro através de diretrizes claras:
</p>

<ul>
  <li>
    <strong>Consentimento:</strong> O tratamento de dados exige a autorização expressa
    do usuário, que deve ser informado sobre a finalidade específica da coleta.
  </li>
  <li>
    <strong>Direitos do Titular:</strong> O cidadão pode, a qualquer momento, solicitar
    a exclusão de seus dados, cancelar autorizações prévias ou pedir a transferência
    de suas informações para outro fornecedor.
  </li>
  <li>
    <strong>Dados Sensíveis:</strong> A lei impõe cuidados rigorosos para dados sensíveis
    e informações de crianças e adolescentes.
  </li>
  <li>
    <strong>Transparência:</strong> As empresas devem justificar a necessidade de
    cada dado solicitado (ex: não faz sentido pedir o nome dos pais em uma compra
    comum de varejo).
  </li>
</ul>

<h4>Fiscalização e Agentes de Tratamento</h4>

<p>
  Para garantir o cumprimento da lei, a estrutura conta com órgãos reguladores e
  papéis específicos dentro das organizações:
</p>

<ul>
  <li>
    <strong>ANPD (Autoridade Nacional de Proteção de Dados):</strong> Órgão responsável
    por fiscalizar e aplicar penalidades. As multas podem chegar a 2% do faturamento
    anual da empresa, limitadas a R$ 50 milhões por infração.
  </li>
  <li>
    <strong>Controlador:</strong> Quem toma as decisões sobre o tratamento dos dados.
  </li>
  <li>
    <strong>Operador:</strong> Quem executa o tratamento dos dados em nome do controlador.
  </li>
  <li>
    <strong>Encarregado (DPO):</strong> O profissional que faz a ponte entre a empresa,
    os titulares dos dados e a ANPD.
  </li>
</ul>

<p>
  As empresas são obrigadas a criar planos de contingência e normas de
  governança. Em caso de vazamentos ou acessos indevidos, o incidente deve ser
  comunicado imediatamente à ANPD e aos indivíduos afetados.
</p>

<h3>ISO 27000: Fundamentos e Estrutura</h3>

<p>
  A família <strong>ISO 27000</strong> é o padrão internacional que define as
  diretrizes para o gerenciamento da Segurança da Informação. É importante
  destacar que ela foca na <strong>gestão e governança</strong>, e não na
  descrição de soluções técnicas ou ferramentas específicas. No Brasil, ela é
  adotada como a norma <strong>NBR ISO/IEC 27000</strong>.
</p>

<h4>Divisão da Família ISO</h4>

<p>
  A "família" é composta por diversas normas que se complementam para formar um
  Sistema de Gestão de Segurança da Informação (SGSI):
</p>

<ul>
  <li>
    ISO 27000: Fornece a visão geral, o vocabulário e os termos fundamentais.
  </li>
  <li>
    ISO 27001: Define os requisitos obrigatórios para estabelecer, implementar e
    manter o sistema de gestão. É a norma contra a qual as empresas são
    auditadas para obter certificação.
  </li>
  <li>
    ISO 27002: Funciona como um guia de "Melhores Práticas". Ela detalha como
    implementar os controles sugeridos pela 27001. É o conteúdo base para quem
    busca certificação profissional na área.
  </li>
</ul>

<h4>Os 12 Domínios da ISO 27000</h4>

<p>
  Para organizar a segurança de forma abrangente, a norma divide as tarefas em
  12 áreas fundamentais (domínios). Embora nem todos sejam obrigatórios para
  todas as empresas, eles cobrem todo o ciclo de vida da informação:
</p>

<ol>
  <li>
    <strong>Avaliação de Risco:</strong> Identificação de ameaças e análise do impacto
    no negócio (ex: perda de dados por falha de hardware).
  </li>
  <li>
    <strong>Política de Segurança:</strong> O documento mestre que orienta todas
    as diretrizes da empresa.
  </li>
  <li>
    <strong>Organização da Segurança da Informação:</strong> Estrutura interna para
    gerir a segurança.
  </li>
  <li>
    <strong>Gerenciamento de Recursos:</strong> Inventário e classificação dos ativos
    de informação.
  </li>
  <li>
    <strong>Segurança de Recursos Humanos:</strong> Regras para antes, durante e
    após a contratação de funcionários.
  </li>
  <li>
    <strong>Segurança Física e Ambiental:</strong> Proteção contra acesso físico
    indevido e desastres naturais.
  </li>
  <li>
    <strong>Gerenciamento de Operações e Comunicações:</strong> Controles operacionais
    de redes e sistemas.
  </li>
  <li>
    <strong>Aquisição, Desenvolvimento e Manutenção de Sistemas:</strong> Segurança
    aplicada no ciclo de vida de softwares.
  </li>
  <li>
    <strong>Controle de Acesso:</strong> Restrição de acesso a sistemas e dados apenas
    a pessoas autorizadas.
  </li>
  <li>
    <strong>Gerenciamento de Incidentes:</strong> Como reagir e reportar falhas ou
    ataques.
  </li>
  <li>
    <strong>Gerenciamento de Continuidade de Negócios:</strong> Planos para manter
    a empresa operando após uma crise.
  </li>
  <li>
    <strong>Conformidade:</strong> Garantia de que a empresa segue leis (como a LGPD)
    e regulamentos.
  </li>
</ol>

<h3>A Política de Segurança</h3>

<p>
  A Política de Segurança é o documento mestre que orienta a gestão da segurança
  em uma organização. Ela não se limita a tecnologias, mas define regras de
  comportamento para usuários e administradores, além de especificar requisitos
  técnicos para os sistemas. Para o profissional de TI, a política serve como um
  guia obrigatório: se o documento exige autenticação de dois fatores, o
  desenvolvedor deve obrigatoriamente implementar essa funcionalidade em suas
  aplicações.
</p>

<h4>Elementos da Política de Segurança</h4>

<p>
  Uma política robusta é estruturada em três componentes principais, que variam
  em nível de obrigatoriedade e detalhamento:
</p>

<ul>
  <li>
    <strong>Padrões:</strong> São definições obrigatórias que garantem a consistência
    tecnológica. Estabelecem quais programas, usuários ou critérios específicos a
    empresa deve seguir para manter a rede operacional e segura.
  </li>
  <li>
    <strong>Diretrizes:</strong> São listas de sugestões e boas práticas. Diferente
    dos padrões, são mais flexíveis e geralmente não obrigatórias, servindo para
    orientar como as tarefas podem ser feitas de forma mais eficiente.
  </li>
  <li>
    <strong>Documentos de Procedimento:</strong> São guias detalhados e técnicos.
    Contêm o "passo a passo" da implementação, incluindo instruções minuciosas, gráficos
    e fluxogramas para a execução de tarefas específicas.
  </li>
</ul>

<h4>Aplicação das Normas ISO na Política</h4>

<p>
  A estrutura da família ISO 27000 oferece as ferramentas para validar e
  executar o que foi planejado na política de segurança:
</p>

<ul>
  <li>
    <strong>ISO 27001:</strong> Funciona como uma lista de verificação (checklist).
    A empresa utiliza esta norma para identificar quais objetivos de controle são
    aplicáveis ao seu cenário específico.
  </li>
  <li>
    <strong>ISO 27002:</strong> Oferece o detalhamento técnico e prático. É ela que
    define os controles necessários para que os objetivos traçados na política e
    na ISO 27001 sejam efetivamente alcançados.
  </li>
</ul>

<h3>Estados do Dado e Responsabilidades</h3>

<p>
  Para que a política de segurança seja eficaz e as normas ISO sejam aplicadas
  corretamente, é preciso entender que os dados residem em três estados
  distintos. A segurança deve ser garantida em cada um deles, e diferentes
  equipes de TI compartilham essa responsabilidade:
</p>

<ul>
  <li>
    <strong>Em Transmissão:</strong> Dados que trafegam pela rede. A
    responsabilidade recai sobre a <strong>equipe de segurança de rede</strong>,
    que deve garantir a integridade e confidencialidade durante o trajeto.
  </li>
  <li>
    <strong>Em Processamento:</strong> Dados que estão sendo manipulados ou
    inseridos. A responsabilidade é dos
    <strong>programadores e da equipe de entrada de dados</strong>, que devem
    assegurar que o código e a operação sejam seguros.
  </li>
  <li>
    <strong>Em Armazenamento:</strong> Dados gravados em discos ou nuvem. A
    responsabilidade é da <strong>equipe de infraestrutura e suporte</strong>,
    que cuida do hardware e dos servidores onde as informações repousam.
  </li>
</ul>

<h4>Aplicação Prática e Carreira</h4>

<p>
  As normas ISO fornecem os controles específicos para cada um desses estados.
  Mesmo profissionais que não desejam ser especialistas em segurança interagem
  com dados em processamento ou armazenamento e, por isso, devem seguir
  estritamente a política de segurança da empresa em suas tarefas diárias. Para
  aqueles que buscam se especializar, as <strong
    >certificações de mercado</strong
  > (como as da família ISO ou CISSP) são diferenciais decisivos em processos seletivos,
  validando a capacidade técnica para proteger dados em qualquer um dos três estados.
</p>
