<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Introdução aos Conceitos de Segurança</h2>

<Audios modulo="M11" aulas={["01", "02", "03", "04"]} />

<p>
  A segurança é um conceito presente desde a infância, inicialmente focado na
  forma de agir para evitar danos físicos (<strong>segurança pessoal</strong>).
  No cotidiano adulto, expande-se para a preservação de bens (<strong
    >segurança patrimonial</strong
  >), como o ato de trancar portas e janelas. Ambas as dimensões possuem medidas
  distintas: a pessoal é regida por normas (como as NRs no trabalho) e
  supervisão técnica, enquanto a patrimonial utiliza dispositivos como alarmes e
  barreiras físicas.
</p>

<p>
  Com a digitalização das interações humanas, esses conceitos são transpostos
  para os sistemas computacionais. A <strong>segurança digital</strong> surge para
  proteger as ações e dados em um mundo onde o trabalho, o estudo e o lazer dependem
  de dispositivos conectados. Para implementá-la, é necessário compreender as características
  do ambiente digital e os modelos de proteção desenvolvidos para esse cenário.
</p>

<h3>O Mundo Digital e a Evolução Tecnológica</h3>

<p>
  A evolução tecnológica alterou a forma como a sociedade se comunica e consome
  serviços. O acesso à educação, por exemplo, deixou de ser restrito
  geograficamente devido à digitalização de materiais e à transmissão de aulas
  em tempo real. Da mesma forma, as redes sociais transformaram as relações
  interpessoais, aproximando pessoas distantes, embora tragam novos desafios de
  isolamento físico. O funcionamento desse ecossistema digital baseia-se em três
  pilares principais para a execução de tarefas e acesso a conteúdos:
</p>

<ul>
  <li>
    <strong>Dispositivos:</strong> Computadores ou smartphones utilizados pelo usuário.
  </li>
  <li><strong>Conexão:</strong> Meios de transmissão de dados (internet).</li>
  <li>
    <strong>Infraestrutura de Armazenamento:</strong> Servidores onde residem os
    dados e as aplicações.
  </li>
</ul>

<p>
  A garantia de segurança em todos esses processos exige a aplicação de
  tecnologias específicas sobre cada componente da comunicação. Compreender como
  esses elementos interagem é o passo fundamental para identificar as
  vulnerabilidades e aplicar as soluções de proteção adequadas.
</p>

<h3>A Rede e a Evolução da Insegurança</h3>

<p>
  A internet é a infraestrutura base que interliga dispositivos para estudo,
  lazer e trabalho. Por ser uma <strong>rede pública</strong>, os dados
  transmitidos através dela podem, em tese, ser capturados por qualquer outro
  dispositivo conectado. Essa característica nativa de abertura levanta
  questionamentos fundamentais sobre a confiabilidade das transações e a
  integridade das informações que trafegam pelo meio digital.
</p>

<p>
  Historicamente, a internet não foi projetada com foco em segurança. Em sua
  origem acadêmica, o objetivo era o compartilhamento livre de documentos e
  mensagens (e-mail) entre universidades. Nessa fase, a prioridade era a
  acessibilidade e a troca de informações, sem mecanismos de restrição ou
  proteção robustos, uma vez que o ambiente era restrito a pesquisadores e
  instituições de ensino.
</p>

<p>
  A necessidade de segurança tornou-se crítica com a entrada das empresas no
  ambiente digital e, principalmente, com o surgimento do <strong
    >e-commerce</strong
  >. A transição de simples trocas de mensagens para transações financeiras e de
  negócios exigiu a proteção de dados sensíveis, como credenciais de acesso e
  números de cartões de crédito. Esse cenário transformou a segurança digital em
  um requisito essencial para garantir a legitimidade dos sites e a prevenção de
  fraudes.
</p>

<h3>O Modelo Cliente/Servidor</h3>

<p>
  O modelo <strong>cliente/servidor</strong> é a base da comunicação nas redes
  digitais e na internet. Ele classifica os dispositivos de acordo com a função
  que exercem no processo: o <strong>cliente</strong> é o dispositivo que
  solicita um serviço ou dado, enquanto o <strong>servidor</strong> é o computador
  onde as aplicações e dados estão hospedados, responsável por atender a essas solicitações.
</p>

<h4>Características do Cliente</h4>

<p>
  O cliente pode ser um computador, tablet ou smartphone. Para interagir com o
  servidor, ele utiliza um aplicativo específico chamado de <strong
    >navegador (browser)</strong
  >
  no caso do acesso à web. Embora muitos sistemas operacionais já tragam navegadores
  nativos, o usuário pode instalar outros de acordo com sua preferência. O cliente
  tem a capacidade de executar diversas aplicações simultaneamente, mantendo conexões
  abertas com diferentes servidores ao mesmo tempo (como e-mail, chat e navegação
  web).
</p>

<h4>Características do Servidor</h4>

<p>
  O servidor geralmente executa uma aplicação específica que deve estar
  constantemente disponível para os clientes. Um exemplo comum é o servidor web,
  que utiliza o protocolo <strong>HTTP</strong> para processar e responder às requisições
  dos navegadores. O servidor envia a resposta (como o conteúdo de uma página) independentemente
  de qual navegador o cliente esteja utilizando.
</p>

<h3>O Modelo AAA</h3>

<p>
  O modelo <strong>AAA</strong> (Authentication, Authorization, Accounting) é um
  framework fundamental para o controle de acesso em sistemas de segurança digital.
  Sua finalidade é orientar a implementação de mecanismos que garantam que apenas
  usuários legítimos acessem dados e recursos específicos, mantendo o registro de
  suas ações.
</p>

<h4>Autenticação (Authentication)</h4>

<p>
  A autenticação é o processo inicial que visa verificar se o usuário é
  realmente quem ele diz ser. Geralmente ocorre através da solicitação de
  credenciais (nome e senha) que são comparadas com um banco de dados de
  usuários autorizados. A identificação baseia-se em três fatores:
</p>

<ul>
  <li><strong>O que o usuário sabe:</strong> Senhas ou números PIN.</li>
  <li>
    <strong>O que o usuário possui:</strong> Dispositivos físicos, tokens ou smartphones
    para recebimento de códigos (SMS/E-mail).
  </li>
  <li>
    <strong>O que o usuário é:</strong> Características biométricas, como impressão
    digital ou reconhecimento facial.
  </li>
</ul>

<p>
  Sistemas modernos priorizam a <strong
    >autenticação de dois fatores (2FA)</strong
  >, que combina dois desses elementos (ex: senha + código por SMS) para elevar
  o nível de segurança.
</p>

<h4>Autorização (Authorization)</h4>

<p>
  Após a confirmação da identidade, a autorização define o que o usuário tem
  permissão para fazer e quais informações pode acessar. Esse controle é
  frequentemente baseado no <strong>perfil ou grupo</strong> do usuário,
  gerenciado por servidores de diretório, como o
  <strong>Active Directory (AD)</strong>. Um exemplo prático é uma rede social:
  você tem autorização para editar suas fotos, enquanto outros usuários têm
  apenas autorização para visualizá-las.
</p>

<h4>Auditoria (Accounting)</h4>

<p>
  A auditoria consiste no registro (log) de todas as atividades realizadas,
  serviços acessados e recursos consumidos durante a sessão. O termo original,
  Accounting (contabilização), reforça a ideia de rastreabilidade. Esse processo
  é essencial para gerar históricos de transações, como em sites de e-commerce,
  permitindo que o usuário ou o administrador verifique datas, horários e ações
  executadas em caso de contestações ou monitoramento.
</p>

<h3>A Tríade CIA</h3>

<p>
  Enquanto o modelo AAA foca no controle de acesso, a <strong>Tríade CIA</strong
  >
  (Confidentiality, Integrity, Availability/Authenticity) foca na proteção e na garantia
  da qualidade dos dados em si. Os dois modelos são complementares.
</p>

<h4>Confidencialidade (Confidentiality)</h4>

<p>
  A confidencialidade garante que os dados sejam acessíveis apenas por pessoas
  ou sistemas autorizados.
</p>

<ul>
  <li>
    <strong>Implementação:</strong> Utiliza os mecanismos de autenticação e autorização
    (do modelo AAA).
  </li>
  <li>
    <strong>Criptografia:</strong> É a principal ferramenta para proteger dados que
    trafegam na internet. Ela codifica a informação de modo que, mesmo se um hacker
    capturá-la, não conseguirá lê-la. O ícone do "cadeado" no navegador indica que
    a comunicação está criptografada.
  </li>
</ul>

<h4>Integridade (Integrity)</h4>

<p>
  A integridade assegura que a informação não foi alterada, seja de forma
  acidental ou proposital, durante o armazenamento ou a transmissão.
</p>

<ul>
  <li>
    <strong>Dados Armazenados:</strong> Garante que o que foi recuperado é exatamente
    o que foi gravado.
  </li>
  <li>
    <strong>Dados Transmitidos:</strong> Garante que o que o destinatário recebeu
    é exatamente o que o emissor enviou.
  </li>
  <li>
    <strong>Mecanismo HASH:</strong> A integridade é verificada através de funções
    matemáticas chamadas Hash, que geram um "resumo" único da mensagem. Se o conteúdo
    mudar, o resumo também muda, alertando sobre a alteração.
  </li>
</ul>

<h4>Autenticidade (Authenticity)</h4>

<p>
  A autenticidade valida a identidade do emissor da informação, garantindo a
  origem dos dados (quem enviou é realmente quem diz ser).
</p>

<ul>
  <li>
    <strong>Assinatura Digital:</strong> Funciona como uma assinatura em papel, mas
    para o meio digital.
  </li>
  <li>
    <strong>Certificados Digitais e CAs:</strong> A validade das assinaturas é
    garantida pelas <strong>Autoridades Certificadoras (CAs)</strong>, que
    funcionam como "cartórios digitais".
  </li>
  <li>
    <strong>Aviso de Certificado Inválido:</strong> Ocorre quando o navegador não
    consegue confirmar a autenticidade do site com uma CA, o que pode indicar um
    risco, embora nem sempre signifique que o site é malicioso.
  </li>
</ul>

<h3>Conclusão: Segurança de Ponta a Ponta</h3>

<p>
  A segurança digital não deve se limitar apenas aos dados em trânsito; ela deve
  abranger todos os elementos do processo de comunicação: o <strong
    >terminal do cliente</strong
  >, os <strong>elementos de rede</strong> e os <strong>servidores</strong>.
</p>

<ul>
  <li>
    <strong>Vulnerabilidade do Cliente:</strong> Mesmo que um servidor seja seguro
    e os dados estejam criptografados, um computador de usuário desprotegido funciona
    como uma "porta aberta" para ataques enquanto estiver conectado à rede pública.
  </li>
  <li>
    <strong>Segurança no Servidor (Modelo AAA):</strong> A proteção do servidor é
    garantida pela validação rigorosa de credenciais (Autenticação), controle de
    permissões por perfil (Autorização) e registro completo de operações (Auditoria).
  </li>
  <li>
    <strong>Segurança dos Dados (Modelo CIA):</strong> A proteção da informação em
    si é feita através da criptografia (Confidencialidade), do uso de resumos matemáticos/Hash
    (Integridade) e de assinaturas ou certificados digitais (Autenticidade).
  </li>
</ul>

<h4>Resumo Comparativo: AAA vs. CIA</h4>

<ul>
  <li>
    <strong>AAA</strong>
    <ul>
      <li>
        <strong>Foco Principal:</strong>
        Controle de Acesso e Gestão de Usuários
      </li>
      <li>
        <strong>Mecanismos Chaves:</strong>
        Senhas, 2FA, Biometria, Perfis de Acesso (AD) e Logs de Auditoria.
      </li>
    </ul>
  </li>
  <li>
    <strong>CIA</strong>
    <ul>
      <li>
        <strong>Foco Principal:</strong>
        Proteção e Confiabilidade do Dado
      </li>
      <li>
        <strong>Mecanismos Chaves:</strong>
        Criptografia, Algoritmos de Hash e Certificados Digitais.
      </li>
    </ul>
  </li>
</ul>
