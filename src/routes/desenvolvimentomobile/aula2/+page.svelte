<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>O Papel dos Frameworks no Desenvolvimento</h2>

<Audios modulo="M9" aulas={["05", "06", "07", "08"]} />

<p>
  Um framework funciona como uma estrutura de suporte que oferece ferramentas,
  bibliotecas e padrões prontos para acelerar a criação de um aplicativo. Em vez
  de escrever todo o código do zero, o desenvolvedor utiliza essa base para
  garantir que o software siga padrões de mercado e funcione corretamente em
  diferentes dispositivos.
</p>

<h3>Pluralidade de Tecnologias</h3>

<p>
  Não existe uma tecnologia única ou absoluta no mercado mobile. O cenário atual
  é composto por diversas abordagens que se misturam, permitindo que diferentes
  linguagens de programação (como JavaScript, Dart ou C#) sejam utilizadas para
  atingir o mesmo objetivo: criar aplicativos funcionais. A escolha de uma
  ferramenta geralmente depende da experiência da equipe, do custo e da
  performance desejada.
</p>

<h3>Ecossistema Baseado em Node.js</h3>

<p>
  Muitas soluções modernas de desenvolvimento mobile utilizam o <strong
    >Node.js</strong
  > como motor. Ele permite que o computador execute código JavaScript fora do navegador,
  servindo como base para a instalação de ferramentas, gerenciamento de pacotes e
  automação de tarefas. Entender esse ecossistema é fundamental para quem deseja
  trabalhar com tecnologias multiplataforma.
</p>

<h4>Características das Abordagens Atuais</h4>

<ul>
  <li>
    <strong>Interoperabilidade:</strong> Capacidade de misturar diferentes tecnologias
    e bibliotecas dentro de um mesmo projeto.
  </li>
  <li>
    <strong>Escalabilidade:</strong> Frameworks facilitam o crescimento do aplicativo
    e a manutenção do código a longo prazo.
  </li>
  <li>
    <strong>Agilidade:</strong> O uso de componentes pré-moldados reduz o tempo de
    lançamento do produto no mercado.
  </li>
</ul>

<h3>O Ecossistema de Execução e Gerenciamento</h3>

<p>
  Para que tecnologias web funcionem como aplicativos, é necessária uma base de
  execução que conecte o código ao sistema operacional.
</p>

<ul>
  <li>
    <strong>Engine de Execução:</strong> Ferramentas baseadas em JavaScript utilizam
    motores (como o V8) para permitir que o código seja interpretado e executado
    fora do navegador tradicional, criando a estrutura do aplicativo.
  </li>
  <li>
    <strong>Gerenciadores de Pacotes (NPM):</strong> São ferramentas essenciais que
    automatizam a instalação e atualização de bibliotecas e utilitários. Eles permitem
    que o desenvolvedor baixe componentes prontos para uso no projeto.
  </li>
  <li>
    <strong>Interface de Linha de Comando (CLI):</strong> É o painel de controle
    do desenvolvedor. Através de comandos de texto no terminal, é possível criar,
    testar e compilar o aplicativo de forma automatizada.
  </li>
</ul>

<h4>Fluxo de Criação e Execução</h4>

<p>
  O desenvolvimento moderno segue um padrão de automação para facilitar o início
  de novos projetos:
</p>

<ul>
  <li>
    <strong>Scaffolding (Estruturação):</strong> Comandos iniciais permitem escolher
    modelos pré-definidos (como navegação por abas ou menus laterais). Isso evita
    que o desenvolvedor perca tempo configurando a arquitetura básica do zero.
  </li>
  <li>
    <strong>Ambiente de Teste Local:</strong> Durante o desenvolvimento, o aplicativo
    é executado em um servidor local. Isso permite visualizar o comportamento da
    aplicação em tempo real no navegador ou em simuladores antes de enviá-lo para
    um dispositivo físico.
  </li>
  <li>
    <strong>Diretórios e Navegação:</strong> Cada aplicativo reside em sua própria
    pasta, onde toda a lógica, estilos e configurações são armazenados e gerenciados.
  </li>
</ul>

<h3>Desenvolvimento em Tempo Real e Depuração</h3>

<p>
  A produtividade no desenvolvimento mobile é impulsionada por recursos de
  feedback imediato:
</p>

<ul>
  <li>
    <strong>Live Reload (Atualização em Tempo Real):</strong> Ao salvar alterações
    no editor de código, o ambiente de teste atualiza automaticamente. Isso permite
    ver o resultado de mudanças em designs ou funções instantaneamente.
  </li>
  <li>
    <strong>Identificação de Erros:</strong> Quando o código contém falhas críticas,
    a tela de visualização geralmente indica o erro ou fica em branco, sinalizando
    que a lógica precisa de correção antes de prosseguir.
  </li>
  <li>
    <strong>Editores de Código:</strong> O uso de editores leves e extensíveis é
    o padrão da indústria, permitindo gerenciar os arquivos do projeto e o terminal
    de comandos em uma interface única.
  </li>
</ul>

<h3>Componentização e Reaproveitamento de Código</h3>

<p>
  No desenvolvimento moderno, as interfaces são construídas através de
  <strong>componentes</strong>. Um componente é um bloco de código reutilizável
  que pode exibir informações diferentes dependendo dos parâmetros que recebe
  (como os nomes "Aluno" ou "Secretaria"). Isso facilita a manutenção, pois você
  altera a estrutura em um único lugar e o comportamento se replica por todo o
  app.
</p>

<h3>Estrutura de Navegação por Abas (Tabs)</h3>

<p>
  A navegação por abas é um dos padrões de interface mais comuns em dispositivos
  móveis. Ela organiza a hierarquia do aplicativo em seções principais
  acessíveis rapidamente.
</p>

<ul>
  <li>
    <strong>Slot:</strong> Define o posicionamento visual de elementos (como colocar
    a barra de navegação no topo ou no rodapé da tela).
  </li>
  <li>
    <strong>Botão de Aba (Tab-Button):</strong> Conecta um ícone e um rótulo de texto
    a uma rota ou página específica.
  </li>
  <li>
    <strong>Ícones e Rótulos:</strong> São elementos visuais fundamentais para a
    usabilidade, ajudando o usuário a identificar a função de cada seção sem precisar
    ler extensos textos.
  </li>
</ul>

<h3>Ciclo de Feedback no Desenvolvimento</h3>

<p>
  A prática de alterar o código HTML e observar a mudança imediata no navegador
  (ou simulador) consolida o fluxo de trabalho de um desenvolvedor mobile.
</p>

<ul>
  <li>
    <strong>Customização:</strong> Pequenas mudanças em tags de texto e propriedades
    de ícones são a base para transformar um modelo padrão (template) em um produto
    personalizado.
  </li>
  <li>
    <strong>Validação:</strong> Testar cada alteração individualmente permite identificar
    erros de sintaxe ou de lógica visual antes que o projeto se torne complexo demais.
  </li>
</ul>
