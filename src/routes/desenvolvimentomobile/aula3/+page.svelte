<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Fundamentos da Documentação e Atualização</h2>

<Audios modulo="M9" aulas={["09", "10", "11", "12"]} />

<p>
  O desenvolvimento mobile é dinâmico, e as ferramentas evoluem rapidamente. Por
  isso, a documentação oficial da tecnologia escolhida deve ser sempre a fonte
  primária de consulta. Depender de tutoriais estáticos pode ser arriscado, pois
  comandos e padrões de projeto tornam-se obsoletos em pouco tempo.
</p>

<h3>Ecossistema de Frameworks (Angular, React e Vue)</h3>

<p>
  Frameworks multiplataforma permitem o uso de diferentes bibliotecas de
  interface para gerenciar a lógica do aplicativo.
</p>

<ul>
  <li>
    <strong>Angular, React e Vue:</strong> São as bases mais comuns para o desenvolvimento
    híbrido. Cada um possui pontos fortes e fracos, mas a escolha muitas vezes baseia-se
    na preferência da equipe ou nos requisitos específicos do projeto, não havendo
    uma "vantagem absoluta" de um sobre o outro.
  </li>
  <li>
    <strong>CLI (Interface de Linha de Comando):</strong> Ferramenta essencial para
    automatizar a criação, teste e compilação do aplicativo através de comandos de
    texto.
  </li>
</ul>

<h3>Gerenciamento de Instalação via NPM</h3>

<p>
  O gerenciamento de dependências é feito por meio de comandos que preparam o
  ambiente de trabalho.
</p>

<ul>
  <li>
    <strong>Instalação Global (-g):</strong> Permite que uma ferramenta (como o Angular
    ou o CLI da plataforma) fique disponível para todo o sistema operacional, evitando
    a necessidade de reinstalá-la a cada novo projeto.
  </li>
  <li>
    <strong>Processo de Download:</strong> Os comandos de instalação costumam demorar,
    pois baixam pacotes de códigos e bibliotecas externas necessários para a execução
    do app.
  </li>
  <li>
    <strong>Alertas vs. Erros:</strong> Durante a instalação, é comum surgirem
    avisos (<strong>WARN</strong>) sobre versões obsoletas ou vulnerabilidades
    leves. Esses alertas não impedem o funcionamento, ao contrário dos erros (<strong
      >ERR</strong
    >), que travam o processo e exigem intervenção técnica ou reinstalação.
  </li>
</ul>

<h3>Padronização entre Sistemas Operacionais</h3>

<p>
  Embora o desenvolvimento possa ocorrer em Linux, Windows ou macOS, os comandos
  de terminal e os resultados finais tendem a ser padronizados. Pequenas
  diferenças, como o uso de comandos de permissão (ex: sudo), são específicas do
  sistema operacional e não alteram a lógica final da aplicação móvel.
</p>

<h3>Inicialização Automatizada (Scaffolding)</h3>

<p>
  A criação de um aplicativo moderno raramente começa do zero absoluto.
  Utiliza-se um processo de <strong>scaffolding</strong> (andaime), disparado por
  comandos no terminal, que guia o desenvolvedor através de configurações iniciais.
</p>

<ul>
  <li>
    <strong>Agilidade:</strong> Esse processo automatiza a estrutura de pastas e
    arquivos de configuração, economizando horas de trabalho manual.
  </li>
  <li>
    <strong>Configuração Visual:</strong> Algumas ferramentas abrem interfaces no
    navegador para facilitar a escolha de recursos, como sistemas de autenticação
    e integração com nuvem, antes mesmo da primeira linha de código ser escrita.
  </li>
  <li>
    <strong>Dinamicidade:</strong> As telas e opções de configuração mudam frequentemente
    conforme as atualizações das ferramentas, por isso o foco deve ser no entendimento
    da lógica do projeto, e não na memorização de telas específicas.
  </li>
</ul>

<h3>Modelos de Layout (Templates)</h3>

<p>
  Ao iniciar um projeto mobile, o desenvolvedor escolhe uma estrutura base de
  interface que dita como o usuário irá navegar pelo app:
</p>

<ul>
  <li>
    <strong>Tabs (Guias):</strong> Layout focado em navegação inferior, ideal para
    alternar entre as funcionalidades principais rapidamente.
  </li>
  <li>
    <strong>Side Menu (Menu Lateral):</strong> Estrutura "gaveta" (hambúrguer), comum
    para aplicativos com muitas seções ou configurações.
  </li>
  <li>
    <strong>Blank (Vazio):</strong> Um projeto limpo para quando se deseja criar
    uma interface totalmente personalizada desde o início.
  </li>
</ul>

<h3>Ciclo de Desenvolvimento e Visualização</h3>

<p>
  O fluxo de trabalho mobile é dividido em etapas de teste, sendo a execução no
  navegador a mais rápida e comum durante a fase de construção:
</p>

<ul>
  <li>
    <strong>Servidor Local (Localhost):</strong> O comando de execução cria um servidor
    temporário que permite visualizar o app no navegador. Isso facilita a depuração
    (debug) e o ajuste de layouts em tempo real.
  </li>
  <li>
    <strong>Visualização Real-Time:</strong> Através do recurso de Live Reload, qualquer
    alteração salva no código é refletida instantaneamente na visualização, permitindo
    um desenvolvimento fluido.
  </li>
  <li>
    <strong>Emuladores e Dispositivos:</strong> Embora o navegador seja o ponto de
    partida, o teste final deve ser feito em emuladores (simuladores de celular no
    PC) ou aparelhos físicos para validar o desempenho e o acesso ao hardware.
  </li>
</ul>

<h3>O Ambiente de Desenvolvimento (IDE)</h3>

<p>
  Para traduzir conceitos em código funcional, utiliza-se um ambiente de
  desenvolvimento especializado. O <strong>VS Code</strong> é o padrão da indústria
  por ser leve e permitir a visualização de toda a árvore de arquivos do projeto
  mobile de forma organizada.
</p>

<ul>
  <li>
    <strong>Acesso Rápido:</strong> O uso de comandos de terminal (como code .) para
    abrir o editor diretamente na pasta do projeto agiliza a transição entre a configuração
    da infraestrutura e a escrita de código.
  </li>
  <li>
    <strong>Visão do Projeto:</strong> Ao abrir o editor, o desenvolvedor tem acesso
    à estrutura completa: pastas de lógica, arquivos de estilo (CSS), marcação (HTML)
    e configurações de plataforma.
  </li>
</ul>

<h3>Fluxo de Trabalho Integrado</h3>

<p>
  O desenvolvimento mobile eficiente baseia-se na execução simultânea de duas
  ferramentas:
</p>

<ol>
  <li>
    <strong>O Editor de Código:</strong> Onde as mudanças lógicas e visuais são realizadas.
  </li>
  <li>
    <strong>O Servidor de Visualização:</strong> Onde o aplicativo é executado em
    tempo real (geralmente via navegador ou emulador).
  </li>
</ol>

<p>
  Essa integração permite o <strong>desenvolvimento iterativo</strong>, onde
  cada linha de código alterada pode ser validada instantaneamente. Entender
  essa dinâmica é fundamental para qualquer tecnologia mobile, pois reduz o
  tempo entre a criação de uma funcionalidade e a correção de eventuais erros.
</p>

<h3>Estrutura de Arquivos e Organização</h3>

<p>
  Independentemente da tecnologia escolhida, um projeto mobile moderno
  organiza-se em diretórios que separam as responsabilidades:
</p>

<ul>
  <li>
    <strong>Código-fonte:</strong> Onde reside a inteligência e as telas do app.
  </li>
  <li>
    <strong>Ativos (Assets):</strong> Pasta destinada a imagens, ícones e fontes.
  </li>
  <li>
    <strong>Configurações de Build:</strong> Arquivos que determinam como o projeto
    será compilado para Android ou iOS.
  </li>
</ul>
