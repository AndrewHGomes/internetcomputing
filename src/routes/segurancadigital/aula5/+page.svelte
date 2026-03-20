<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Protocolos de Comunicação e o Modelo TCP/IP</h2>

<Audios modulo="M11" aulas={["17", "18", "19", "20"]} />

<p>
  A comunicação na internet baseia-se no modelo <strong>TCP/IP</strong>, uma
  estrutura de quatro camadas utilizada por todos os dispositivos da rede. No
  processo padrão de acesso a um site, o computador (cliente) utiliza o
  protocolo <strong>HTTP</strong> (Hypertext Transfer Protocol) para solicitar e
  receber dados de um servidor. Esse tráfego é transportado pelos protocolos
  <strong>TCP</strong>
  (transporte) e <strong>IP</strong> (internet).
</p>

<h4>Camadas e Protocolos de Segurança</h4>

<p>
  A segurança digital não é universal para todas as aplicações; cada tipo de
  serviço (e-mail, jogos, navegação) exige soluções específicas. Como a
  navegação web é a atividade mais comum, o foco recai sobre como proteger as
  mensagens trocadas entre cliente e servidor. No modelo TCP/IP, a segurança é
  implementada em diferentes camadas através de protocolos específicos:
</p>

<ul>
  <li>
    <strong>Camada de Aplicação:</strong> Onde opera o <strong>HTTPS</strong>, a
    versão segura do HTTP.
  </li>
  <li>
    <strong>Camada de Transporte:</strong> Onde operam o <strong>SSL</strong>
    (Secure Sockets Layer) e o <strong>TLS</strong> (Transport Layer Security).
  </li>
</ul>

<h3>O Modelo CIA na Comunicação</h3>

<p>
  Para que uma comunicação seja considerada verdadeiramente segura, os
  protocolos devem garantir os pilares do modelo <strong>CIA</strong>:
</p>

<ol>
  <li>
    <strong>Confidencialidade:</strong> Garante que apenas o destinatário autorizado
    leia a mensagem.
  </li>
  <li>
    <strong>Integridade:</strong> Assegura que a mensagem não foi alterada durante
    o trajeto.
  </li>
  <li>
    <strong>Autenticidade:</strong> Confirma a identidade das partes envolvidas (quem
    diz ser o remetente realmente o é).
  </li>
</ol>

<p>
  Além do HTTPS e TLS/SSL, a segurança também pode ser reforçada através de <strong
    >VPNs</strong
  >
  (Virtual Private Networks), que criam conexões protegidas em redes públicas.
</p>

<h3>O Protocolo HTTPS</h3>

<p>
  O <strong>HTTPS</strong> (HyperText Transfer Protocol Secure) é a versão segura
  do protocolo de comunicação da web. Enquanto o HTTP padrão transmite dados em texto
  aberto — permitindo que informações sensíveis, como senhas e cartões de crédito,
  sejam interceptadas por hackers —, o HTTPS protege a comunicação através da criptografia.
</p>

<h4>Diferenças Técnicas e Portas</h4>

<p>
  A distinção entre os protocolos ocorre já na camada de transporte por meio de
  suas portas lógicas:
</p>

<ul>
  <li>
    <strong>HTTP:</strong> Opera na porta 80. É considerado inseguro por não criptografar
    o conteúdo.
  </li>
  <li><strong>HTTPS:</strong> Opera na porta 443.</li>
</ul>

<p>
  Para administradores de rede, essa diferenciação é vital: é possível
  configurar um <strong>Firewall</strong> para bloquear a porta 80 e permitir apenas
  a 443, obrigando todos os usuários a utilizarem exclusivamente a navegação segura.
</p>

<h4>Identificação Visual</h4>

<p>
  A segurança de uma conexão HTTPS é sinalizada diretamente no navegador do
  usuário. Os principais indicadores são:
</p>

<ul>
  <li>
    A presença de um ícone de <strong>cadeado</strong> ao lado do endereço.
  </li>
  <li>O prefixo https:// no início da URL.</li>
</ul>

<h4>O Papel da Criptografia</h4>

<p>
  O HTTPS não atua sozinho para garantir a segurança. Ele utiliza protocolos
  complementares, como o <strong>TLS/SSL</strong>, para realizar a criptografia
  das mensagens. Esse processo garante o pilar da
  <strong>confidencialidade</strong>: mesmo que os dados sejam capturados
  durante o trajeto, eles estarão codificados e serão ilegíveis para invasores.
</p>

<h3>Os Protocolos SSL e TLS</h3>

<p>
  Os protocolos <strong>SSL</strong> (Secure Sockets Layer) e
  <strong>TLS</strong> (Transport Layer Security) são os responsáveis diretos pela
  criptografia no modelo HTTPS. Eles garantem que, mesmo que um hacker intercepte
  as mensagens, o conteúdo permaneça codificado e ilegível.
</p>

<h4>Histórico e Evolução</h4>

<ul>
  <li>
    <strong>SSL:</strong> Criado pela Netscape em 1990. Tornou-se o padrão de segurança
    da internet em 1996 (na versão 3.0).
  </li>
  <li>
    <strong>TLS:</strong> É a evolução direta do SSL. A partir da versão 3.1 do SSL,
    o protocolo foi renomeado para TLS 1.0.
  </li>
  <li>
    <strong>Uso Atual:</strong> Devido a vulnerabilidades descobertas no SSL ao
    longo dos anos, o <strong>TLS</strong> é o protocolo recomendado e utilizado
    atualmente, embora o termo "SSL/TLS" ainda seja usado comercialmente para se
    referir a ambos.
  </li>
</ul>

<h4>Funcionamento do SSL/TLS</h4>

<p>
  O processo de estabelecimento de uma conexão segura ocorre basicamente em duas
  etapas principais:
</p>

<ol>
  <li>
    <strong>Autenticação:</strong> O servidor envia seu
    <strong>certificado digital</strong>
    ao cliente. O cliente utiliza um padrão de chave pública (<strong
      >PKCS</strong
    >) para validar se o servidor é autêntico.
  </li>
  <li>
    <strong>Criptografia (Troca de Chaves):</strong> Cliente e servidor negociam
    quais algoritmos de codificação serão usados e compartilham a
    <strong>chave de criptografia</strong>. Esta chave é o elemento crítico: sem
    ela, o invasor não consegue decifrar os dados capturados.
  </li>
</ol>

<h4>Estrutura do TLS</h4>

<p>O protocolo TLS é dividido em duas camadas funcionais:</p>

<ul>
  <li>
    <strong>TLS Handshake Protocol:</strong> Responsável pela autenticação entre
    as partes e pela negociação dos algoritmos e chaves de criptografia.
  </li>
  <li>
    <strong>TLS Record Protocol:</strong> Camada que efetivamente implementa a
    criptografia dos dados transmitidos (utilizando algoritmos como o
    <strong>DES - Data Encryption Standard</strong>).
  </li>
</ul>

<h3>O Certificado Digital</h3>

<p>
  O <strong>Certificado Digital</strong> atua como uma "carteira de identidade"
  de um site ou servidor. Sua função principal é garantir a
  <strong>autenticidade</strong>, provando ao navegador que o site é realmente
  quem diz ser antes de iniciar uma conexão segura.
</p>

<h4>Autoridades Certificadoras (CA)</h4>

<p>
  Para que um certificado seja confiável, ele deve ser emitido por uma
  <strong>Autoridade Certificadora (CA)</strong>.
</p>

<ul>
  <li>
    O processo é análogo a um documento oficial: assim como a Secretaria de
    Segurança Pública valida um RG, a CA valida a identidade digital de um
    servidor.
  </li>
  <li>
    Ao acessar um site HTTPS, o navegador do cliente consulta a CA indicada no
    certificado para verificar sua legitimidade.
  </li>
</ul>

<h4>Criptografia Assimétrica e Chaves</h4>

<p>
  Após a validação do certificado, o servidor fornece sua <strong
    >chave pública</strong
  >
  para estabelecer a confidencialidade dos dados. O modelo utiliza o conceito de
  <strong>chaves assimétricas</strong>:
</p>

<ul>
  <li>
    <strong>Chave Pública:</strong> Disponibilizada pelo site para que o navegador
    do cliente criptografe as informações enviadas.
  </li>
  <li>
    <strong>Chave Privada:</strong> Mantida em segredo absoluto pelo servidor. É
    a única capaz de descriptografar os dados selados pela chave pública correspondente.
  </li>
</ul>

<p>
  Mesmo que um hacker intercepte os dados no caminho, ele não conseguirá lê-los,
  pois não possui a chave privada necessária para a decodificação.
</p>

<ol>
  <li><strong>Acesso:</strong> O cliente acessa o site via HTTPS.</li>
  <li>
    <strong>Identificação:</strong> O servidor envia seu Certificado Digital.
  </li>
  <li>
    <strong>Validação:</strong> O cliente verifica o certificado junto à Autoridade
    Certificadora.
  </li>
  <li>
    <strong>Criptografia:</strong> O cliente usa a chave pública do servidor para
    codificar os dados (como senhas ou dados bancários).
  </li>
  <li>
    <strong>Recebimento:</strong> O servidor usa sua chave privada para ler as informações.
  </li>
</ol>

<h3>Redes Privadas Virtuais (VPN)</h3>

<p>
  A <strong>VPN</strong> (Virtual Private Network) é uma tecnologia que permite criar
  uma rede privada e segura utilizando uma infraestrutura pública e insegura, como
  a Internet. O conceito de "virtual" refere-se ao fato de os dados trafegarem como
  se estivessem em uma rede exclusiva, graças ao uso de criptografia.
</p>

<h4>O Mecanismo de Tunelamento</h4>

<p>
  O funcionamento básico da VPN baseia-se no <strong>tunelamento</strong>. Assim
  como no HTTPS, os dados são criptografados antes do envio, criando um "túnel"
  de proteção que impede que terceiros interceptem ou compreendam a informação
  durante o trajeto.
</p>

<h4>Tipos de VPN</h4>

<p>
  Existem duas formas principais de implementar esses túneis, dependendo da
  necessidade de conexão:
</p>

<ul>
  <li>
    <strong>Site-to-Site (Local a Local):</strong> Conecta duas redes completas (ex:
    a matriz e uma filial de uma empresa). A configuração é feita diretamente nos
    roteadores ou Firewalls/UTMs de ambas as pontas. Para os usuários, a sensação
    é de que todos os computadores estão no mesmo prédio físico.
  </li>
  <li>
    <strong>Client-to-Site (Cliente a Local):</strong> Conecta um dispositivo individual
    a uma rede corporativa. É o modelo comum para trabalho remoto (home office).
    O usuário utiliza um software específico (cliente VPN) no seu computador ou smartphone
    para estabelecer a conexão segura com o servidor da empresa.
  </li>
</ul>

<h4>Implementação e Soluções de Mercado</h4>

<p>
  A escolha da ferramenta de VPN deve estar alinhada à política de segurança da
  instituição. Existem diversas soluções comerciais e de código aberto, como:
</p>

<ul>
  <li><strong>OpenVPN</strong> (amplamente utilizado e flexível).</li>
  <li>
    <strong>Forticlient</strong> (Fortinet), <strong>Cisco</strong>,
    <strong>Check</strong> <strong>Point</strong> e
    <strong>AWS Client VPN</strong>.
  </li>
</ul>

<p>
  Essas aplicações exigem configurações prévias, como o endereço IP de destino e
  credenciais de acesso, para garantir que apenas usuários autorizados
  estabeleçam o túnel.
</p>

<h3>Conclusão: Fluxo da Navegação Segura e Boas Práticas</h3>

<p>
  Este trecho recapitula como os elementos de segurança (HTTPS, SSL/TLS,
  Certificados e VPN) trabalham em conjunto para garantir a proteção dos dados e
  introduz cuidados essenciais que o usuário deve tomar.
</p>

<h4>O Processo de Conexão Segura</h4>

<p>
  Mesmo que um usuário tente acessar um site via <strong>HTTP</strong>
  (inseguro), a maioria dos servidores modernos realiza o redirecionamento automático
  para o <strong>HTTPS</strong>. O fluxo de proteção ocorre da seguinte forma:
</p>

<ol>
  <li>
    <strong>Criptografia:</strong> O protocolo SSL/TLS define os parâmetros de segurança
    e codifica as mensagens do HTTP antes que elas sejam encapsuladas nos pacotes
    IP para trafegar pela internet.
  </li>
  <li>
    <strong>Identificação:</strong> A chave necessária para essa criptografia é
    extraída do <strong>Certificado Digital</strong> enviado pelo site.
  </li>
  <li>
    <strong>Validação:</strong> A Entidade Certificadora atua como um terceiro de
    confiança, validando o certificado para garantir que o site é legítimo (autenticidade).
  </li>
</ol>

<h4>Fator Humano e Prevenção de Fraudes</h4>

<p>
  A tecnologia protege o caminho dos dados, mas não impede que o usuário acesse
  voluntariamente um site malicioso.
</p>

<ul>
  <li>
    <strong>Verificação de URL:</strong> É fundamental conferir se o endereço na
    barra do navegador é realmente o pretendido.
  </li>
  <li>
    <strong>Cuidado com Links:</strong> Nunca acesse sites sensíveis (bancos, sistemas
    corporativos) através de links recebidos por e-mail, pois podem levar a sites
    falsos (phishing) desenhados para roubar dados, mesmo que apresentem um cadeado
    de segurança.
  </li>
</ul>

<h4>Conectividade Corporativa (VPN)</h4>

<p>
  Para o trabalho remoto, a <strong>VPN</strong> estende essa segurança para toda
  a comunicação com a rede da empresa.
</p>

<ul>
  <li>
    Cria um <strong>túnel criptografado</strong> que garante a confidencialidade.
  </li>
  <li>
    Exige uma solução de software específica no computador do usuário que deve
    ser compatível com a infraestrutura da empresa.
  </li>
</ul>
