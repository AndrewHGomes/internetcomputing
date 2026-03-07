<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Estrutura de Redes e Comunicação</h2>

<Audios modulo="M10" aulas={["05", "06", "07", "08"]} />

<p>
  Uma rede de computadores consiste em um conjunto de dispositivos
  interconectados que compartilham dados e se comunicam entre si. Essa
  integração entre computação e comunicação transformou a organização dos
  sistemas modernos, permitindo a troca global de informações
</p>

<p>
  A infraestrutura de uma rede é composta por elementos físicos e dispositivos
  eletônicos. Os <strong>meios de ligação</strong>
  incluem cabos (como o par trançado e a fibra óptica) ou tecnologias sem fio (como
  o Wi-Fi, que utiliza ondas de rádio). Já os
  <strong>dispositivos dedicados</strong> são responsáveis por definir as rotas e
  encaminhar as mensagens da origem ao destino.
</p>

<h4>Componentes Principais da Rede</h4>

<ul>
  <li>
    <strong>Roteadores:</strong>
    Dispositivos que encaminham pacotes de dados entre diferentes redes, escolhendo
    a melhor rota.
  </li>
  <li>
    <strong>Switches:</strong>
    Conectam dispositivos em uma mesma rede local, entregando os dados especificamente
    ao destino correto.
  </li>
  <li>
    <strong>Hubs:</strong>
    Equipamentos mais simples que retransmitem os dados recebidos para todos os dispositivos
    conectados à rede.
  </li>
  <li>
    <strong>Cabos de Rede:</strong>
    Meios físicos para transmissão de sinais elétricos ou luminosos.
  </li>
  <li>
    <strong>Ondas de Rádio:</strong>
    Meio de transmissão para conexões sem fio.
  </li>
</ul>

<p>
  A rede funciona como a arquitetura de base para o acesso à internet. Sem essa
  estrutura física e lógica de encaminhamento de tráfego, a comunicação e o
  acesso aos serviços web seriam impossíveis.
</p>

<h3>Tipos de Redes e Modelos de Referência</h3>

<p>
  A conexão entre um usuário e uma página web é estabelecida através de links
  (URLs), que funcionam como pontes para as redes. Essas redes são classificadas
  de acordo com sua abrangência geográfica:
</p>

<ul>
  <li>
    <strong>LAN (Local Area Network):</strong>
    Redes locais que interligam dispositivos em um mesmo espaço físico, como uma
    residência ou escritório.
  </li>
  <li>
    <strong>MAN (Metropilitan Area Network):</strong>
    Redes metropolitanas que conectam dispositivos a alguns quilômetros de distância,
    como escritórios diferentes em uma mesma cidade.
  </li>
  <li>
    <strong>WAN (Wide Area Network):</strong>
    Redes de longa distância que abrangem grandes áreas, como países ou continentes.
  </li>
</ul>

<h4>Modelos de Referência</h4>

<p>
  Os modelos de referência são estruturas conceituais que padronizam a
  comunicação entre dispositivos de diferentes fabricantes. Eles garantem que os
  dados enviados por um sistema possam ser interpretados por outro.
</p>

<h4>Modelo OSI (7 Camadas)</h4>

<p>
  Criado pela ISO, este modelo divide a comunicação em sete etapas distintas
  para organizar a padronização dos protocolos:
</p>

<ol>
  <li>
    <strong>Física:</strong>
    Transmissão bruta de bits por meios físicos (cabos, rádios).
  </li>
  <li>
    <strong>Enlace de Dados:</strong>
    Controla o fluxo e a sequência dos dados enviados.
  </li>
  <li>
    <strong>Rede:</strong>
    Responsável pelo roteamento dos pacotes da origem ao destino.
  </li>
  <li>
    <strong>Transporte:</strong>
    Divide os dados em unidades menores e garante que cheguem corretamente.
  </li>
  <li>
    <strong>Sessão:</strong>
    Gerencia a eficiência da comunicação entre aplicações.
  </li>
  <li>
    <strong>Apresentação:</strong>
    Atua como tradutor, lidando com sintaxe, criptografia e compressão.
  </li>
  <li>
    <strong>Aplicação:</strong>
    Interface direta com o usuário final e seus programas.
  </li>
</ol>

<h4>Modelo TCP/IP (4 Camadas)</h4>

<p>
  É o modelo prático utilizado na internet moderna. Ele simplifica a estrutura
  do OSI ao agrupar funções de sessão e apresentação na camada superior:
</p>

<ul>
  <li>
    <strong>Aplicação:</strong>
    Onde operam protocolos como HTTP.
  </li>
  <li>
    <strong>Transporte:</strong>
    Utiliza protocolos como <strong>TCP</strong> (entrega segura) e
    <strong>UDP</strong> (transmissão rápida).
  </li>
  <li>
    <strong>Internet:</strong>
    Realiza o endereçamento e roteamento via protocolo <strong>IP</strong>.
  </li>
  <li>
    <strong>Acesso à Rede:</strong>
    Gerencia a transmissão física dos dados pelo hardware (ex: Wi-Fi, Ethernet).
  </li>
</ul>

<h3>Protocolos de Rede</h3>

<p>
  Os protocolos de rede são conjuntos de regras e padrões que permitem a
  comunicação entre diferentes dispositivos. Eles garantem que a troca de dados
  ocorra de forma idêntica, segura e efiente, independentemente da localização
  geográfica, do fabricante do hardware ou do sistema operacional utilizado. Sem
  essa padronização, a comunicação entre dispositivos distintos da rede seria
  impossível.
</p>

<h4>Principais Protocolos e suas Funções</h4>

<p>
  Abaixo estão listados os protocolos fundamentais para o funcionamento da
  internet e dos serviços web:
</p>

<ul>
  <li>
    <strong>TCP/IP:</strong>
    Combinação do TCP (transmissão e controle de dados) com o IP (roteamento de pacotes).
    É a base da comunicação na internet.
  </li>
  <li>
    <strong>HTTP:</strong>
    Protocolo padrão para transferência de dados e páginas na Web (WWW).
  </li>
  <li>
    <strong>HTTPS:</strong>
    Versão segura do HTTP que utiliza camadas de criptografia (SSL/TLS) para proteger
    as informações.
  </li>
  <li>
    <strong>FTP:</strong>
    Protocolo especializado na transferência de arquivos entre computadores na rede.
  </li>
  <li>
    <strong>SMTP:</strong>
    Protocolo padrão utilizado especialmente para o envio de mensagens de e-mail.
  </li>
  <li>
    <strong>DNS:</strong>
    Funciona como uma lista telefônica da rede, traduzindo nomes de domínios (URLs)
    em endereços IP.
  </li>
  <li>
    <strong>SSL/TLS:</strong>
    Protocolos de segurança que fornecem criptografia para as comunicações, garantindo
    a privacidade dos dados.
  </li>
  <li>
    <strong>UDP:</strong>
    Protocolo de transporte de dados mais leve e rápido que o TCP, ideal para transmissões
    que toleram pequenas perdas, como streaming de vídeo e jogos onlilne.
  </li>
</ul>

<h3>Configuração de Servidor Local</h3>

<p>
  Para testar aplicações web antes de publicá-las na internet (sem um domínio
  real), desenvolvedores utilizam ambientes de servidor local. Essas ferramentas
  agrupam todos os componentes necessários para o desenvolvimento, testes e
  depuração em um único pacote instalado no próprio computador. As duas
  principais aplicações para essa finalidade são:
</p>

<ul>
  <li>
    <strong>XAMPP:</strong>
    Ferramenta de código aberto que inclui servidor Apache, o banco de dados MariaDB
    e supporte para scripts em PHP. É multiplataforma.
  </li>
  <li>
    <strong>WAMPP:</strong>
    Semelhante ao XAMPP em funcionalidades, mas desenvolvido especificamente para
    o sistema operacional Windows.
  </li>
</ul>

<h4>Instalação do XAMPP</h4>

<p>
  A instalação deve ser feita preferencialmente pelo site oficial (<strong
    >apachefriends.org</strong
  >). O usuário deve escolher a versão mais recente compatível com seu sistema
  operacional, atentando-se para a versão do PHP incluída no pacote.
</p>

<p>
  O processo de instalação no Windows segue o padrão simplificado: após o
  arquivo baixado, basta avançar pelas etapas confirmando as opções padrão até a
  conclusão do assistente.
</p>

<h3>Utilização e Teste do XAMPP</h3>

<p>
  Para iniciar o servidor local, o usuário deve abrir o Painel de Controle do
  XAMPP e ativar os serviços necessários (geralmente <strong>Apache</strong> e
  <strong>MySQL/MariaDB</strong>) clicando no botão <strong>Start</strong>.
  Quando o serviço é iniciado com sucesso, o botão muda para
  <strong>Stop</strong> e o status de funcionamento é exibido na interface.
</p>

<h4>Verificação de Funcionamento</h4>

<p>
  A validação de que o sevidor local está operante é feita diretamente pelo
  navegador web (Chrome, Edge, Firefox, etc.). O procedimento consiste em:
</p>

<ul>
  <li>
    Digitar <strong>localhost</strong> na barra de endereços (URL) e pressionar Enter.
  </li>
  <li>
    Se os serviços estiverem configurados corretamente, o navegador carregará a
    página de boas-vindas oficial do XAMPP (Dashboard).
  </li>
</ul>

<p>
  Essa página confirma que o ambiente está pronto para hospedar e testar
  arquivos de código web localmente, antes de qualquer publicação em um servidor
  real.
</p>

<h3>Conclusão: Redes e Servidores Web</h3>

<p>
  Esta etapa consolidou o entendimento sobre a infraestrutura necessária para a
  existência da web, desde a conexão física até a lógica de transmissão de
  dados. O conhecimento foi estruturado em três pilares: classificação de redes,
  modelos de referência e ferramentas de desenvolvimento local.
</p>

<h4>Classificação e Estrutura de Redes</h4>

<p>
  As redes são categorizadas pela sua abrangência geográfica, definindo como os
  dispositivos se conectam em diferentes escalas:
</p>

<ul>
  <li>
    <strong>LAN:</strong> Redes locais de curto alcance (ex: residências e escritórios).
  </li>
  <li>
    <strong>MAN:</strong> Redes metropolitanas que conectam áreas dentro de uma mesma
    cidade.
  </li>
  <li>
    <strong>WAN:</strong> Redes de longa distância que interligam países e continentes.
  </li>
</ul>

<h4>Modelos de Referência e Protocolos</h4>

<p>
  A comunicação entre dispositivos de diferentes fabricantes é garantida pela
  padronização através de modelos de camadas:
</p>

<ul>
  <li>
    <strong>Modelo OSI:</strong> Estrutura teórica de 7 camadas que detalha todo
    o processo de comunicação.
  </li>
  <li>
    <strong>Modelo TCP/IP:</strong> Estrutura prática de 4 camadas utilizada na internet
    moderna.
  </li>
  <li>
    <strong>Protocolos:</strong> Regras essenciais como
    <strong>HTTP/HTTPS</strong>
    (web), <strong>FTP</strong> (arquivos),
    <strong>SMTP</strong> (e-mail) e <strong>DNS</strong> (resolução de nomes).
  </li>
</ul>

<h4>Servidores Web e Desenvolvimento Local</h4>

<p>
  Para o desenvolvimento e teste de aplicações, utilizam-se servidores locais
  que emulam o ambiente da internet no computador do desenvolvedor:
</p>

<ul>
  <li>
    <strong>XAMPP e WAMP:</strong> Pacotes que instalam Apache, MySQL/MariaDB e PHP
    de forma integrada.
  </li>
  <li>
    <strong>Localhost:</strong> Endereço utilizado no navegador para acessar e validar
    o funcionamento do servidor local após a ativação dos serviços no painel de controle.
  </li>
</ul>
