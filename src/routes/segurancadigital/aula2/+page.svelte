<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Analogia entre Segurança Real e Digital</h2>

<Audios modulo="M11" aulas={["05", "06", "07", "08"]} />

<p>
  A segurança digital pode ser compreendida pela comparação com a segurança
  patrimonial. No mundo virtual, as <strong>ameaças</strong> são indivíduos
  mal-intencionados (frequentemente chamados de hackers) que buscam se apropriar
  de ativos alheios. Assim como um ladrão segue uma sequência de ações para
  invadir uma casa (quebrar um vidro, destravar a janela, entrar), os ataques
  digitais possuem uma <strong>sequência de operações características</strong>.
  O estudo dessas etapas é fundamental para a adoção de medidas preventivas
  eficazes.
</p>

<h3>Dispositivos e Arquitetura de Rede</h3>

<p>
  A forma como um ataque ocorre e as características das ameaças dependem
  diretamente do tipo de dispositivo visado. Na comunicação via internet, os
  dispositivos são classificados em duas categorias principais:
</p>

<ul>
  <li>
    <strong>Dispositivos Finais (Terminais):</strong> São os pontos de origem ou
    destino da comunicação. Exemplos incluem computadores, servidores, impressoras,
    câmeras IP, smartphones, tablets e dispositivos IoT (Internet das Coisas).
  </li>
  <li>
    <strong>Dispositivos Intermediários:</strong> São responsáveis por conectar os
    dispositivos finais e interligar diferentes redes para formar a internet. Exemplos
    incluem switches (conexão via cabo), Access Points (conexão Wi-Fi) e roteadores
    (interconexão de redes locais com a rede externa).
  </li>
</ul>

<h3>Integração de Funções em Ambientes Domésticos</h3>

<p>
  Em redes residenciais, é comum que as funções de vários dispositivos
  intermediários estejam integradas em um único equipamento fornecido pelo
  provedor de internet. Esse aparelho costuma desempenhar simultaneamente os
  papéis de:
</p>

<ul>
  <li><strong>Access Point (AP):</strong> Para conexões sem fio.</li>
  <li><strong>Switch:</strong> Para conexões via cabo de rede.</li>
  <li>
    <strong>Roteador:</strong> Para estabelecer a comunicação entre a rede interna
    da residência e a rede externa (internet).
  </li>
</ul>

<h3>Conceito de Malware</h3>

<p>
  As ameaças que visam dispositivos finais (computadores, smartphones e
  servidores) são genericamente chamadas de <strong>Malwares</strong>. A
  classificação desses códigos maliciosos baseia-se em dois critérios
  principais: o seu <strong>mecanismo de atuação</strong> e o seu
  <strong>modo de propagação</strong>.
</p>

<h4>Principais Tipos de Malwares</h4>

<p>A lista de ameaças comuns inclui:</p>

<ul>
  <li>Vírus</li>
  <li>Worms</li>
  <li>Cavalos de Troia</li>
  <li>Bomba lógica</li>
  <li>Ransomware</li>
  <li>Backdoors e Rootkits</li>
</ul>

<h3>Diferenças entre Vírus e Worms</h3>

<h4>Vírus</h4>

<p>
  O vírus é um arquivo executável que necessita de um <strong>hospedeiro</strong
  >
  (outro arquivo ou programa) para se propagar. Sua principal característica é a
  dependência da
  <strong>ação do usuário</strong>: o código malicioso só causa danos quando o
  usuário executa o programa infectado. A prevenção básica consiste em evitar
  arquivos de fontes desconhecidas ou não confiáveis.
</p>

<h4>Worms</h4>

<p>
  Diferente dos vírus, os <strong>Worms</strong> não precisam de interação humana
  ou de um arquivo hospedeiro para se espalhar. Eles exploram vulnerabilidades e
  falhas de segurança diretamente nos sistemas, o que os torna consideravelmente
  mais perigosos e destrutivos.
</p>

<p>
  A medida de proteção mais eficaz contra Worms é manter todos os sistemas e
  softwares <strong>atualizados</strong>, pois as atualizações corrigem as
  brechas exploradas. O uso de softwares piratas aumenta o risco, já que estes
  não recebem tais correções oficiais.
</p>

<h4>Cavalo de Troia (Trojan)</h4>

<p>
  Funciona como um veículo de transporte para outros códigos maliciosos. Ele se
  oculta dentro de um programa aparentemente inofensivo ou útil, como jogos
  gratuitos e utilitários. A infecção ocorre quando o usuário executa o arquivo.
  A principal prevenção é <strong>
    não utilizar softwares de fontes desconhecidas ou piratas
  </strong>.
</p>

<h4>Bomba Lógica</h4>

<p>
  É um código programado para ser executado apenas quando um gatilho específico
  é acionado, como uma <strong>data, hora ou evento do sistema</strong>. Sua
  presença é silenciosa e difícil de detectar até que o mecanismo de disparo
  "exploda" o comando malicioso.
</p>

<h4>Ransomware</h4>

<p>
  É um ataque de "sequestro" de dados. O invasor utiliza criptografia para
  tornar os arquivos do usuário inacessíveis e exige o pagamento de um <strong
    >resgate</strong
  >
  (geralmente em criptomoedas como Bitcoin para evitar rastreamento) em troca da
  chave de decriptação. Um exemplo histórico famoso é o Wannacry.
</p>

<h4>Backdoors e Rootkits</h4>

<p>Ambos visam garantir o acesso persistente do invasor ao sistema:</p>

<ul>
  <li>
    <strong>Backdoor:</strong> Cria uma "porta dos fundos" que ignora sistemas de
    proteção (como Firewalls), permitindo que o invasor assuma o controle total do
    computador com os privilégios do usuário.
  </li>
  <li>
    <strong>Rootkit:</strong> É um conjunto de ferramentas que altera o núcleo do
    sistema operacional para esconder a presença de invasores e assegurar a abertura
    de backdoors.
  </li>
</ul>

<p>
  <strong>Prevenção</strong>: A melhor defesa contra essas ameaças é a
  combinação de <strong> manter o sistema operacional atualizado </strong> (para
  corrigir vulnerabilidades) e
  <strong>não executar arquivos de procedência duvidosa</strong>.
</p>

<h3>Mecanismos de Ataque (Engenharia Social)</h3>

<p>
  Os ataques buscam enganar o usuário para obter informações pessoais,
  credenciais bancárias ou dados de cartões de crédito. Eles são classificados
  conforme o canal e a estratégia de abordagem:
</p>

<h4>Phishing</h4>

<p>
  É o método mais comum, onde o criminoso envia mensagens falsas (geralmente via
  e-mail) fingindo ser uma instituição confiável, como um banco ou uma loja. O
  objetivo é atrair o usuário para um site falso que imita o original. Ao
  digitar seus dados, o usuário os entrega diretamente ao invasor. Exemplos
  comuns incluem solicitações de "atualização cadastral" ou promoções com preços
  muito abaixo do mercado.
</p>

<h4>Spear Phishing</h4>

<p>
  Uma variação personalizada e direcionada do Phishing. O atacante utiliza
  informações específicas do alvo (coletadas em redes sociais, por exemplo),
  como nome e hábitos de consumo, para tornar a mensagem mais verossímil e
  aumentar as chances de sucesso do golpe.
</p>

<h4>Vishing</h4>

<p>
  Adaptado para a tecnologia de voz (VoIP), este ataque utiliza mensagens de
  áudio ou chamadas telefônicas. O criminoso simula uma gravação automática de
  uma instituição financeira para solicitar a confirmação de dados confidenciais
  por voz.
</p>

<h4>Pharming</h4>

<p>
  Refere-se à criação e utilização do site falso que imita o legítimo. Como o
  invasor não pode usar o domínio exato do site oficial, ele utiliza endereços
  muito parecidos. A principal medida de prevenção é <strong>
    verificar atentamente a URL (nome do site) na barra de endereços do
    navegador
  </strong>. Se houver qualquer divergência no nome oficial, a navegação deve
  ser interrompida imediatamente.
</p>

<h3>Softwares Antivírus</h3>

<p>
  O antivírus é a ferramenta básica de proteção contra malwares. Seu
  funcionamento é comparável a uma vacina: ele analisa os arquivos do sistema em
  busca de <strong>assinaturas</strong> (sequências de código) que correspondam a
  padrões de vírus já conhecidos e estudados.
</p>

<h4>Funcionamento e Atualização</h4>

<p>
  Para ser eficaz, o antivírus precisa ser <strong
    >periodicamente atualizado</strong
  >. Como hackers criam novas ameaças ou modificam códigos antigos
  constantemente, o software só conseguirá identificar novos perigos se sua base
  de dados de "vírus conhecidos" estiver em dia. Atualmente, essas ferramentas
  também são capazes de identificar e bloquear a ação de <strong>Worms</strong>.
</p>

<h3>Recomendações de Uso</h3>

<ul>
  <li>
    <strong>Não desabilite a proteção:</strong> O escaneamento de arquivos em tempo
    real pode reduzir levemente a velocidade do computador, mas desativá-lo deixa
    o sistema totalmente vulnerável.
  </li>
  <li>
    <strong>Sistemas Integrados:</strong> Sistemas operacionais modernos (como o
    Windows 10 e superiores) já possuem antivírus nativos (ex: Windows Defender),
    eliminando a necessidade de instalações extras se o usuário preferir.
  </li>
  <li>
    <strong>Proteção em Dispositivos Móveis:</strong> Smartphones também são alvos
    de ataques e devem possuir softwares de proteção instalados.
  </li>
  <li>
    <strong>Versões Gratuitas:</strong> Caso o sistema não possua uma ferramenta
    nativa, recomenda-se a instalação de um antivírus mesmo que em sua versão gratuita,
    pois é preferível à ausência total de proteção.
  </li>
</ul>

<h3>Conclusão: Revisão de Malwares e Defesa</h3>

<p>
  O cenário de ameaças digitais exige vigilância constante, pois a evolução dos
  dispositivos acompanha a sofisticação dos ataques:
</p>

<ul>
  <li>
    <strong>Vírus:</strong> Embora conhecidos, ainda exigem atenção. Causam
    lentidão e danos aos dados, demandando o uso de antivírus inclusive em
    <strong>smartphones</strong>.
  </li>
  <li>
    <strong>Worms:</strong> Mantêm-se como ameaças críticas devido à sua automação,
    mas podem ser barrados por antivírus modernos que reconhecem seus padrões de
    código.
  </li>
  <li>
    <strong>Cavalos de Troia e Backdoors:</strong> O Cavalo de Troia serve para
    enganar o usuário e "pular" o <strong>Firewall</strong>. Uma vez executado,
    ele pode abrir um Backdoor, permitindo que o invasor acesse não apenas o
    dispositivo infectado, mas toda a rede interna segura.
  </li>
</ul>

<h3>O Fator Humano na Segurança</h3>

<p>
  A segurança digital não depende exclusivamente de tecnologia de ponta, mas sim
  de um <strong>processo contínuo</strong> que envolve:
</p>

<ul>
  <li>
    <strong>Atualização Constante:</strong> Manter sistemas e ferramentas de proteção
    em dia para mitigar novas variantes de ataques.
  </li>
  <li>
    <strong>Comportamento do Usuário:</strong> Ações inseguras podem anular os recursos
    tecnológicos mais sofisticados. Ter o melhor "alarme" (software) é inútil se
    o usuário esquecer de "ligá-lo" ou facilitar a entrada da ameaça por meio de
    práticas negligentes.
  </li>
</ul>

<h3>Recomendações Finais de Proteção</h3>

<ul>
  <li>
    <strong>Mantenha o Firewall e o Antivírus ativos:</strong> Eles são a primeira
    linha de defesa contra acessos externos não autorizados.
  </li>
  <li>
    <strong>Atenção à execução de arquivos:</strong> O Cavalo de Troia depende da
    sua ação para abrir as portas do sistema.
  </li>
  <li>
    <strong>Conscientização:</strong> A ferramenta técnica é apenas metade da solução;
    a postura preventiva do usuário completa a segurança.
  </li>
</ul>
