<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Segurança e Armazenamento na Web</h2>

<Audios modulo="M10" aulas={["09", "10", "11", "12"]} />

<p>
  A segurança em plataformas web é o pilar fundamental para proteger a
  privacidade dos usuários e a integridade de informações sensíveis. Dados
  pessoais e financeiros circulam constantemente pela rede; sem mecanismos de
  proteção adequados, esses ativos ficam vulneráveis a acessos não autorizados,
  o que pode resultar em fraudes financeiras e roubo de identidade. As ameaças
  às aplicações web geralmente surgem de três fontes principais:
</p>

<ul>
  <li>
    <strong>Falhas de codificação:</strong>
    Erros na escrita do código que geram brechas.
  </li>
  <li>
    <strong>Configurações de servidores:</strong>
    Servidores mal ajustados que expõem portas ou dados desnecessários.
  </li>
  <li>
    <strong>Design da aplicação:</strong>
    Problemas estruturais na lógica de como o sistema funciona.
  </li>
</ul>

<p>
  Hackers exploram essas vulnerabilidades para aplicar golpes como
  <strong>ransomware</strong> (sequestro de dados) e outras fraudes online. Por isso,
  a segurança não deve ser um recurso adicional, mas sim uma prioridade pensada em
  todas as etapas do ciclo de vida do software: desde o planejamento inicial e desenvolvimento
  até a fase de produção, quando a aplicação está disponível para o público final.
</p>

<h3>Conceitos Fundamentais de Segurança da Informação</h3>

<p>
  A segurança da informação busca proteger sistemas e dados contra ameaças,
  garantindo a confiança do usuário e a continuidade dos serviços. Para que uma
  aplicação seja considerada segura, ela deve implementar quatro pilares
  essenciais:
</p>

<ul>
  <li>
    <strong>Confidencialidade:</strong>
    Garante que a informação seja acessível apenas por pessoas ou sistemas autorizados.
    O principal mecanismo de proteção aqui é a
    <strong>criptografia</strong>, que codifica os dados para que apenas quem
    possui a chave correta consiga lê-los.
  </li>
  <li>
    <strong>Integridade:</strong>
    Assegura que os dados não foram alterados de forma indevida ou acidental. Utiliza-se
    a técnica de <strong>hashing</strong>, que gera um código único para o dado;
    se o dado mudar, o código muda, revelando a alteração.
  </li>
  <li>
    <strong>Disponibilidade:</strong>
    Garante que o sistema e os dados estejam acessíveis sempre que o usuário precisar.
    Para evitar interrupções (como ataques DoS), utilizam-se redundâncias, balanceamento
    de carga e planos de recuperação.
  </li>
  <li>
    <strong>Autenticidade:</strong>
    Valida a identidade de quem acessa o sistema, garantindo que as partes são quem
    dizem ser. É implementada através de senhas, certificados digitais e autenticação
    de dois fatores (2FA).
  </li>
</ul>

<h3>Criptografia e seus Tipos</h3>

<p>
  A criptografia é o processo de converter informações em um formato codificado,
  garantindo que apenas quem possui a
  <strong>chave de acesso</strong> possa lê-las. Ela é essencial para a segurança
  web, protegendo a confidencialidade e a integridade tanto no armazenamento local
  quanto no tráfego de dados pela internet.
</p>

<h4>Criptografia Simétrica</h4>

<p>
  Utiliza a <strong>mesma chave</strong> para codificar e decodificar a informação.
  É eficiente para os dados armazenados onde apenas o proprietário tem a chave, mas
  apresenta limitações de segurança em comunicações de rede (devido ao risco no compartilhamento
  da chave única).
</p>

<ul>
  <li>
    <strong>AES:</strong>
    Padrão atual, altamente seguro e eficiente.
  </li>
  <li>
    <strong>DES:</strong>
    Antigo e atualmente considerado inseguro.
  </li>
  <li>
    <strong>3DES:</strong>
    Versão que aplica o DES três vezes para aumentar a robustez.
  </li>
</ul>

<h4>Criptografia Assimétrica</h4>

<p>
  Utiliza um par de chaves distinto: uma <strong>chave pública</strong> (que
  pode ser compartilhada com qualquer pessoa para criptografar) e uma
  <strong>chave privada</strong> (mantida em segredo pelo dono para descriptografar).
  É a base da segurança na internet (HTTPS) e de aplicativos de mensagens com criptografia
  ponta a ponta.
</p>

<ul>
  <li>
    <strong>RSA:</strong>
    Amplamente usado em assinaturas digitais e comunicação web.
  </li>
  <li>
    <strong>ECC:</strong>
    Oferece alta segurança com chaves menores, resultando em melhor desempenho que
    o RSA.
  </li>
</ul>

<h4>Criptografia Híbrida</h4>

<p>
  Combina os dois anteriores para aproveitar a velocidade da simétrica com a
  segurança na troca de chaves da assimétrica. Na prática, a criptografia
  assimétrica é usada para trocar uma chave simétrica de forma segura; uma vez
  estabelecida, os dados passam a ser transmitidos via criptografia simétrica.
</p>

<ul>
  <li>
    <strong>Exemplo (SSL/TLS):</strong>
    Quando você acessa um site via <strong>HTTPS</strong>, o navegador e o
    servidor realizam um <strong>handshake</strong>. Eles usam chaves públicas
    (assimétrica) para combinar uma chave comum (simétrica), que será usada para
    proteger o restante da navegação.
  </li>
</ul>

<h3>Servidor Apache e Instalação Básica</h3>

<p>
  O <strong>Apache</strong> é um software de código aberto e modular que atua
  como intermediário entre o navegador do usuário e os conteúdos do servidor.
  Ele é escalável, compatível com diversos sistemas operacionais e suporta
  múltiplas linguagens de programação. Em termos de segurança, oferece suporte
  nativo para <strong>HTTPS (SSL/TLS)</strong>, autenticação de usuários e
  controle de acesso baseado em IP.
</p>

<h4>Processo de Instalação</h4>

<p>
  Para configurar um servidor local com suporte HTTPS, o primeiro passo é a
  instalação manual do Apache no Windows:
</p>

<ol>
  <li>
    <strong>Download:</strong>
    Acesse o site oficial do Apache, navegue até a seção de downloads e selecione
    a opção <strong>Apache Lounge</strong>.
  </li>
  <li>
    <strong>Versão:</strong>
    Escolha a versão compatível com o seu sistema operacional (Win64 ou Win32).
  </li>
  <li>
    <strong>Extração:</strong>
    Extraia os arquivos em um diretório simples, evitando pastas com caracteres especiais
    (exemplo sugerido: C:\Apache).
  </li>
  <li>
    <strong>Configuração de Caminho (Root):</strong>
    <ul>
      <li>Navegue atá a pasta de configuração: C:\Apache\Apache24\conf.</li>
      <li>Abra o arquivo de configuração principal com um editor de texto.</li>
      <li>
        Localize a diretiva <strong>Define SRVROOT</strong> e insira o caminho exato
        onde os arquivos foram extraídos (ex: C:/Apache/Apache24).
      </li>
      <li>Salve e feche o arquivo para validar a alteração.</li>
    </ul>
  </li>
</ol>

<h3>Instalação e Configuração do Apache como Serviço</h3>

<p>
  Após configurar os arquivos de diretório, é necessário registrar e iniciar o
  Apache no Windows utilizando o Prompt de Comando (CMD) com privilégios de
  administrador. O objetivo é transformar o software em um serviço que rode em
  segundo plano.
</p>

<h4>Registro via Terminal (CMD)</h4>

<p>
  Para instalar o serviço, navegue até a pasta binária do Apache seguindo estes
  passos:
</p>

<ul>
  <li>
    <strong>Navegação:</strong>
    Utilize o comando cd .. para retornar à raíz da unidade C:, e então acesse o
    diretório do servidor (ex: cd apache24/bin).
  </li>
  <li>
    <strong>Comando de Instalação:</strong>
    Execute o comando httpd -k install.
  </li>
  <li>
    <strong>Permissão:</strong>
    Caso o Windows exiba um alerta de segurança, é necessário clicar em Permitir
    para autorizar a comunicação do servidor na rede.
  </li>
</ul>

<h4>Ativação do Serviço</h4>

<p>
  Uma vez instalado, o serviço precisa ser iniciado manualmente pela primeira
  vez:
</p>

<ul>
  <li>
    Acesse a ferramenta <strong>Serviços</strong> do Windows (através do menu iniciar).
  </li>
  <li>
    Localize o ítem <strong>Apache</strong> na lista de serviços.
  </li>
  <li>
    Clique com o botão direito e selecione <strong>Iniciar</strong>. O status
    deve mudar para Em execução.
  </li>
</ul>

<h4>Validação do Funcionamento</h4>

<p>
  Para confirmar que o servidor está operando corretamente, realiza um teste de
  conexão local:
</p>

<ul>
  <li>
    Abra o navegador e digite o endereço IP do loopback: <strong
      >127.0.0.1</strong
    >
  </li>
  <li>
    Se a configuração estiver correta, a página exibirá a mensagem padrão <strong
      >Ir Works!</strong
    >, indicando que o navegador conseguiu se comunicar com o servidor Apache
    com sucesso.
  </li>
</ul>

<h3>Conclusão: Segurança e Infraestrutura Web</h3>

<p>
  Concluímos que a segurança e o armazenamento na web são pilares para a
  proteção de dados sensíveis que circulam entre usuários e sistemas. A
  integridade desses dados depende diretamente da implementação correta de
  camadas de proteção para evitar fraudes e acessos não autorizados. Os
  principais pontos revisados foram:
</p>

<ul>
  <li>
    <strong>Importância do Armazenamento Seguro:</strong>
    Garantia de que informações pessoais e financeiras não sejam interceptadas ou
    exploradas por terceiros.
  </li>
  <li>
    <strong>Modelos de Criptografia:</strong>
    <ul>
      <li>
        <strong>Simétrica:</strong> Mesma chave para codificar e decodificar.
      </li>
      <li><strong>Assimétrica:</strong> Par de chaves pública e privada.</li>
      <li>
        <strong>Híbrida:</strong> Uso da força da simétrica com a troca de chaves
        da assimétrica (base do HTTPS).
      </li>
    </ul>
  </li>
  <li>
    <strong>Infraestrutura com Apache:</strong>
    O processo de instalação, registro como serviço no Windows e validação através
    do endereço local 127.0.0.1.
  </li>
</ul>

<h4>Próximos Passos</h4>

<p>
  O foco agora será deslocado da infraestrutura e segurança para o
  desenvolvimento prático. Abordaremos as <strong
    >linguagens de programação</strong
  >, diferenciando as tecnologias que rodam no lado do <strong>cliente</strong>
  (front-end) das que rodam no lado do <strong>servidor</strong> (back-end).
</p>
