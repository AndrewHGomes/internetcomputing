<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Desenvolvimento Baseado em Projetos Reais</h2>

<Audios modulo="M9" aulas={["17", "18", "19", "20"]} />

<p>
  A melhor forma de internalizar o desenvolvimento mobile é criando aplicações
  que resolvam problemas comuns, como uma <strong>Galeria de Fotos</strong>.
  Este tipo de projeto permite explorar o ciclo completo de um app:
</p>

<ul>
  <li>
    <strong>Captura de Dados:</strong> Uso da câmera para entrada de informação.
  </li>
  <li><strong>Exibição:</strong> Organização visual em grades (grids).</li>
  <li>
    <strong>Persistência:</strong> Armazenamento permanente no sistema de arquivos
    do dispositivo, garantindo que os dados não sumam ao fechar o app.
  </li>
</ul>

<h4>Preparação do Ambiente e CLI</h4>

<p>
  O sucesso do desenvolvimento depende de um terminal configurado corretamente.
</p>

<ul>
  <li>
    <strong>Permissões:</strong> No Windows, o uso do terminal como Administrador
    evita bloqueios de escrita. No Mac/Linux, o comando sudo é o recurso para elevar
    privilégios quando ocorrem erros de acesso (root).
  </li>
  <li>
    <strong>Terminal Integrado:</strong> O uso do terminal dentro do próprio editor
    de código (IDE) agiliza o fluxo, embora possa exigir ajustes de segurança em
    algumas máquinas.
  </li>
</ul>

<h4>Plugins de Funcionalidade Nativa</h4>

<p>
  Para que um código escrito em tecnologias web acesse o hardware do celular,
  instalamos bibliotecas específicas que servem de ponte:
</p>

<ul>
  <li>
    <strong>Câmera:</strong> Permite solicitar permissão ao usuário e capturar fotos
    ou vídeos.
  </li>
  <li>
    <strong>Filesystem (Sistema de Arquivos):</strong> Permite ler e gravar arquivos
    diretamente na memória do aparelho.
  </li>
  <li>
    <strong>Preferences (Preferências):</strong> Usado para salvar pequenas quantidades
    de dados, como configurações do usuário, de forma persistente.
  </li>
  <li>
    <strong>PWA Elements:</strong> Componentes que garantem que o aplicativo funcione
    e exiba interfaces de câmera mesmo quando testado em um navegador web, simulando
    o comportamento do celular.
  </li>
</ul>

<h3>Configuração de Ambiente e Estrutura Inicial</h3>

<p>
  O desenvolvimento mobile moderno geralmente começa com a instalação de
  interfaces de linha de comando (CLI) e ferramentas que permitem a comunicação
  entre o código web e as funcionalidades nativas do aparelho (como câmera e
  GPS). Ao iniciar um projeto, é comum utilizar modelos pré-configurados com
  navegação por abas para acelerar o processo e seguir padrões de mercado.
</p>

<p>
  A estrutura do projeto é organizada em pastas onde ficam os arquivos de
  configuração e a lógica da aplicação. O fluxo de trabalho padrão envolve abrir
  o diretório no editor de código e gerenciar dependências específicas para cada
  recurso de hardware que se deseja utilizar no dispositivo móvel.
</p>

<h4>Interface do Usuário (UI) e Hot Reload</h4>

<p>
  A construção da interface baseia-se em componentes visuais que definem
  cabeçalhos, barras de ferramentas e áreas de conteúdo. Um conceito essencial é
  o "Live Reload" ou "Hot Reload", que permite visualizar alterações no código
  instantaneamente no navegador ou dispositivo de teste, otimizando o ciclo de
  desenvolvimento.
</p>

<p>
  Os elementos visuais são customizáveis através de propriedades simples, como
  nomes de ícones, rótulos de botões e posicionamento de elementos flutuantes
  (como botões de ação rápida para captura de mídia).
</p>

<h4>Arquitetura Baseada em Serviços</h4>

<p>
  Para manter o código organizado e reutilizável, utiliza-se o conceito de
  <strong>Serviços</strong>. Em vez de escrever a lógica de acesso ao hardware
  diretamente na tela, cria-se uma classe dedicada (serviço) que encapsula essa
  funcionalidade. Isso facilita a manutenção e permite que diferentes partes do
  aplicativo utilizem o mesmo recurso.
</p>

<h3>Integração com Recursos Nativos</h3>

<p>
  O acesso a funcionalidades de hardware, como a câmera, o sistema de arquivos e
  o armazenamento local, é feito através de pontes de comunicação (plugins). A
  principal vantagem das ferramentas modernas é a abstração: o desenvolvedor
  escreve uma única chamada de método (como tirar uma foto) e o sistema se
  encarrega de executar a ação correta, seja no Android, iOS ou Navegador.
</p>

<h4>Fluxo de Implementação de Funcionalidades:</h4>

<ul>
  <li>
    <strong>Importação:</strong> Adiciona-se as referências das APIs de hardware
    no serviço.
  </li>
  <li>
    <strong>Lógica Assíncrona:</strong> Utiliza-se funções assíncronas para aguardar
    a interação do usuário (como o momento do clique na foto) sem travar o aplicativo.
  </li>
  <li>
    <strong>Injeção de Dependência:</strong> O serviço criado é injetado na página
    desejada através do construtor da classe.
  </li>
  <li>
    <strong>Vinculação (Binding):</strong> Conecta-se a função lógica a um evento
    de clique na interface do usuário para disparar a ação.
  </li>
</ul>

<h3>Modelagem de Dados e Tipagem</h3>

<p>
  Para garantir a organização e a segurança do código, utiliza-se a criação de
  <strong>Models</strong> (Modelos) ou <strong>Interfaces</strong>. Isso define
  a estrutura que um objeto deve ter. No caso de uma galeria, o objeto "Foto"
  precisa armazenar metadados essenciais, como o caminho do arquivo no sistema e
  o caminho para exibição na interface (WebView).
</p>

<h3>Gerenciamento de Coleções (Arrays)</h3>

<p>
  Em vez de manipular uma única imagem, o serviço deve gerenciar uma <strong>
    lista (array)
  </strong> de objetos. Ao capturar uma nova mídia, ela é adicionada a essa coleção.
  O uso de métodos que inserem o novo item no início da lista (como o unshift) garante
  que a foto mais recente seja a primeira a aparecer para o usuário.
</p>

<h4>Renderização Dinâmica de Listas</h4>

<p>
  A exibição de múltiplos itens na tela é feita através de componentes de <strong
  >
    Grid (Grade)
  </strong> e estruturas de repetição (loops). O funcionamento básico consiste em:
</p>

<ul>
  <li>
    <strong>Container de Grade:</strong> Define como o espaço será dividido (ex:
    duas colunas por linha).
  </li>
  <li>
    <strong>Laço de Repetição:</strong> O framework percorre a lista de dados e,
    para cada item encontrado, gera automaticamente um componente visual de imagem.
  </li>
  <li>
    <strong>Vinculação de Caminho (Source Binding):</strong> A origem da imagem na
    tela é vinculada dinamicamente ao caminho armazenado no objeto de dados.
  </li>
</ul>

<h3>Experiência do Usuário (UX)</h3>

<p>
  A separação entre a lógica (serviço) e a visualização (HTML/UI) permite que o
  aplicativo seja atualizado em tempo real. Assim que o dado é inserido na lista
  pelo serviço, a interface reage e renderiza a nova imagem sem a necessidade de
  recarregar a página manualmente.
</p>
