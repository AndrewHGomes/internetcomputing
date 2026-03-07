<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Estrutura e Arquitetura de Projetos</h2>

<Audios modulo="M9" aulas={["13", "14", "15", "16"]} />

<p>
  A base de um aplicativo moderno é dividida em blocos coesos que separam a
  interface da lógica de negócios. Essa organização permite que o mesmo código
  gere experiências consistentes tanto em <strong>iOS</strong> quanto em
  <strong>Android</strong>.
</p>

<ul>
  <li>
    <strong>Módulos:</strong> Funcionam como contêineres que agrupam funcionalidades
    relacionadas, mantendo o projeto organizado e fácil de manter.
  </li>
  <li>
    <strong>Componentes:</strong> São as unidades básicas da interface. Cada elemento
    visual ou funcional da tela é um componente que combina código e lógica.
  </li>
  <li>
    <strong>Templates:</strong> Definem a "visão" do usuário. Utilizam uma linguagem
    baseada em HTML para estruturar o que será exibido na tela.
  </li>
  <li>
    <strong>Serviços:</strong> Classes especializadas em tarefas específicas (como
    buscar dados ou realizar cálculos), que podem ser compartilhadas por várias partes
    do aplicativo.
  </li>
  <li>
    <strong>Ativos (Assets) e Recursos Externos:</strong> Englobam arquivos locais
    (imagens, ícones) e a conexão com o mundo exterior, como bancos de dados e APIs.
  </li>
</ul>

<h3>O Papel do TypeScript e a Transpilação</h3>

<p>
  No desenvolvimento mobile de alto nível, utiliza-se o <strong
    >TypeScript</strong
  > para escrever uma lógica mais robusta e segura.
</p>

<ul>
  <li>
    <strong>Interatividade Complexa:</strong> O TypeScript permite processar dados
    de forma eficiente, garantindo uma melhor experiência para o usuário final.
  </li>
  <li>
    <strong>Transpilação:</strong> Como os navegadores e motores de execução leem
    JavaScript, o código escrito em TypeScript passa por um processo automático de
    "tradução" (transpilação) para a versão de JavaScript compatível com o sistema.
  </li>
  <li>
    <strong>Código Bruto vs. Compilado:</strong> O trabalho do desenvolvedor acontece
    na pasta de origem (src/), onde o código é legível e organizado. O sistema se
    encarrega de transformar esse material no pacote final que o celular consegue
    executar.
  </li>
</ul>

<h3>Integração com o Mundo Exterior</h3>

<p>
  Um aplicativo raramente funciona de forma isolada. A arquitetura deve prever a
  comunicação com recursos externos:
</p>

<ul>
  <li>
    <strong>APIs:</strong> Pontes de comunicação que permitem ao app enviar e receber
    informações de servidores.
  </li>
  <li>
    <strong>JSON:</strong> O formato padrão de troca de dados entre o aplicativo
    e os serviços externos, por ser leve e fácil de processar.
  </li>
</ul>

<h3>Anatomia do Diretório Principal (App)</h3>

<p>
  O coração de um aplicativo multiplataforma reside em uma pasta central que
  organiza toda a lógica, interface e navegação. A separação desses arquivos
  segue o princípio da <strong>responsabilidade única</strong>, facilitando a
  manutenção.
</p>

<ul>
  <li>
    <strong>Ponto de Entrada (Main Component):</strong> É o esqueleto do app. Ele
    gerencia o ciclo de vida inicial, verificando se a plataforma (Android/iOS) e
    os plugins nativos (câmera, GPS, etc.) estão prontos para uso.
  </li>
  <li>
    <strong>Módulo de Roteamento (Routing):</strong> Define as "estradas" do aplicativo.
    É aqui que se configura qual componente deve aparecer quando o usuário clica
    em um botão ou navega para uma nova seção.
  </li>
  <li>
    <strong>Módulo Principal (Main Module):</strong> Funciona como o manifesto do
    projeto, declarando quais componentes e bibliotecas externas fazem parte do ecossistema
    do app.
  </li>
  <li>
    <strong>Estilização Global (Styles):</strong> Arquivos que definem a identidade
    visual (cores, fontes e espaçamentos) que será aplicada em todo o projeto.
  </li>
</ul>

<h3>Organização por Páginas e Componentes</h3>

<p>
  A arquitetura moderna organiza as telas em pastas individuais. Cada página do
  aplicativo geralmente contém quatro arquivos fundamentais:
</p>

<ol>
  <li>
    <strong>Estrutura (HTML/Templates):</strong> O desenho dos elementos na tela.
  </li>
  <li>
    <strong>Lógica (TypeScript/Scripts):</strong> O comportamento daquela tela específica.
  </li>
  <li>
    <strong>Estilo (CSS/Sass):</strong> O visual exclusivo daquela página.
  </li>
  <li>
    <strong>Módulo de Rota:</strong> A configuração de como chegar até aquela tela.
  </li>
</ol>

<h3>Integração com Serviços e Dados Remotos</h3>

<p>
  Dispositivos móveis possuem recursos de processamento e armazenamento
  limitados. Por isso, a arquitetura mobile depende fortemente de serviços
  externos.
</p>

<ul>
  <li>
    <strong>Serviços (Services):</strong> São classes criadas para lidar com tarefas
    pesadas ou compartilhadas, como buscar dados em uma API ou processar geolocalização.
    Ao separar a lógica de processamento da visualização, o código torna-se mais
    leve e reutilizável.
  </li>
  <li>
    <strong>Consumo de Dados:</strong> Quase todas as funções avançadas (mapas, login,
    feeds de notícias) dependem de conexões remotas. O aplicativo atua como uma interface
    que requisita esses dados e os exibe ao usuário.
  </li>
  <li>
    <strong>Integração Nativa (Bridge):</strong> Ferramentas como o Capacitor servem
    como uma ponte, permitindo que o código web acesse funcionalidades físicas do
    celular, como o hardware de GPS para renderizar um mapa.
  </li>
</ul>

<h3>Fluxo de Criação de Novas Telas</h3>

<p>A expansão de um aplicativo segue um fluxo padronizado:</p>

<ul>
  <li>
    <strong>Geração:</strong> Uso de comandos para criar automaticamente a estrutura
    de uma nova página.
  </li>
  <li>
    <strong>Conexão:</strong> Linkar a nova página à tela inicial ou ao menu de navegação.
  </li>
  <li>
    <strong>Execução:</strong> Visualizar as mudanças em tempo real para garantir
    que a transição entre telas e a carga de dados estejam funcionando conforme o
    planejado.
  </li>
</ul>

<h3>Integração com Recursos Nativos (Plugins)</h3>

<p>
  O desenvolvimento mobile moderno utiliza <strong>plugins</strong> para acessar
  funções físicas do aparelho que não estão disponíveis em uma página web comum.
  O uso de mapas é o exemplo clássico de integração entre software e hardware.
</p>

<ul>
  <li>
    <strong>Geolocalização:</strong> O aplicativo obtém coordenadas (latitude e longitude)
    através de múltiplas fontes: GPS (mais preciso), sinais de rede (IP), Wi-Fi,
    Bluetooth ou torres de telefonia (IDs de células GSM).
  </li>
  <li>
    <strong>Gerenciamento de Plugins:</strong> Bibliotecas como o
    <strong>Capacitor</strong> permitem adicionar suporte específico para sistemas
    operacionais diferentes (Android e iOS) através de comandos de instalação, garantindo
    que o código JavaScript consiga "conversar" com as APIs nativas de cada fabricante.
  </li>
</ul>

<h3>O Ciclo de Vida e a Renderização do Mapa</h3>

<p>
  Para que um mapa seja exibido corretamente, o código deve respeitar o tempo de
  carregamento do hardware e da interface:
</p>

<ul>
  <li>
    <strong>Identificação Visual:</strong> No arquivo de estrutura (HTML), define-se
    um contêiner (geralmente uma div) que servirá de âncora para o mapa.
  </li>
  <li>
    <strong>Ações de Ciclo de Vida:</strong> O mapa não deve ser carregado antes
    da tela estar pronta. Utilizam-se eventos como ionViewDidEnter (quando a tela
    entra em foco) para iniciar a criação do mapa e ionViewDidLeave para encerrá-lo,
    economizando memória e bateria do dispositivo.
  </li>
  <li>
    <strong>Configuração Geométrica:</strong> O aplicativo calcula as dimensões reais
    da tela do celular (largura, altura e posição) para desenhar o mapa exatamente
    no espaço disponível.
  </li>
  <li>
    <strong>Customização de Visualização:</strong> É possível definir via código
    o tipo de mapa (normal, satélite, híbrido ou terreno) e o nível de zoom inicial.
  </li>
</ul>

<h3>Testes em Dispositivos Reais</h3>

<p>
  Embora o desenvolvimento ocorra no computador, funcionalidades que dependem de
  hardware (como GPS e Câmera) exigem testes em aparelhos físicos ou emuladores
  configurados.
</p>

<ul>
  <li>
    <strong>ADB (Android Debug Bridge):</strong> Ferramenta essencial para conectar
    o computador ao celular, permitindo instalar e depurar o aplicativo diretamente
    no hardware real.
  </li>
  <li>
    <strong>Permissões:</strong> Aplicativos que acessam localização exigem que o
    desenvolvedor configure permissões de segurança nos arquivos do sistema, garantindo
    que o usuário autorize o acesso aos dados de GPS.
  </li>
</ul>

<h3>Biblioteca de Componentes de Interface (UI)</h3>

<p>
  O desenvolvimento mobile moderno baseia-se no uso de bibliotecas de
  componentes pré-construídos. Esses elementos são projetados para se comportar
  de forma nativa, adaptando visualmente o estilo caso o aplicativo esteja
  rodando em um iPhone (iOS) ou em um dispositivo Android.
</p>

<ul>
  <li>
    <strong>Variedade de Elementos:</strong> Além de mapas, existem componentes para
    quase todas as necessidades comuns, como calendários, seletores de data (date
    pickers), listas expansíveis, modais e cartões de informação.
  </li>
  <li>
    <strong>Documentação Técnica:</strong> O uso de documentações oficiais e guias
    de CLI (Interface de Linha de Comando) é a melhor prática para implementar esses
    componentes, pois eles contêm os trechos de código e as propriedades necessárias
    para customização.
  </li>
  <li>
    <strong>Consistência Visual:</strong> Utilizar componentes padronizados garante
    que o usuário tenha uma experiência familiar e intuitiva, respeitando as diretrizes
    de design de cada sistema operacional.
  </li>
</ul>

<h3>Evolução para Aplicações Complexas: O CRUD</h3>

<p>
  Após dominar a interface e o uso de componentes básicos, o próximo passo no
  desenvolvimento mobile é a criação de aplicações funcionais que manipulam
  dados, conhecidas como <strong>CRUD</strong> (Create, Read, Update, Delete):
</p>

<ul>
  <li>
    <strong>Persistência de Dados:</strong> Envolve a capacidade do aplicativo de
    gravar, ler, atualizar e excluir informações, seja em um banco de dados local
    ou em um servidor remoto.
  </li>
  <li>
    <strong>Manipulação de Mídia:</strong> Funcionalidades avançadas permitem que
    o app interaja com a galeria ou a câmera para processar imagens, armazenando-as
    e exibindo-as conforme a necessidade do usuário.
  </li>
  <li>
    <strong>Lógica de Negócio:</strong> À medida que o app evolui, a
    complexidade aumenta, exigindo uma integração mais profunda entre os
    <strong>Serviços</strong>
    (lógica de dados) e os <strong>Componentes</strong> (visualização).
  </li>
</ul>

<h3>Conclusão</h3>

<p>
  O domínio inicial das ferramentas e da estrutura de pastas prepara o
  desenvolvedor para desafios maiores. A transição de um "app de visualização"
  (como um mapa estático) para um "app de gerenciamento" (com login e
  armazenamento) é o que define um software profissional no mercado mobile.
</p>
