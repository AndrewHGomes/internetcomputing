<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Fundamentos e Arquitetura Web</h2>

<Audios modulo="M10" aulas={["13", "14", "15", "16"]} />

<p>
  O acesso às páginas na internet ocorre através da conversão de uma
  <strong>URL</strong> em um <strong>endereço IP</strong>. O navegador envia uma
  solicitação via protocolo <strong>HTTP</strong> ao servidor, que responde entregando
  o conteúdo solicitado. Esse processo é sustentado por uma arquitetura de redes
  que permite a comunicação entre o usuário e o servidor.
</p>

<h3>Divisão de uma Aplicação Web</h3>

<p>
  O desenvolvimento de sistemas web é estruturado em três pilares que interagem
  entre si para garantir o funcionamento da aplicação.
</p>

<ul>
  <li>
    <strong>Front-end:</strong>
    A interface visual e a parte do código com o qual o usuário interage diretamente.
  </li>
  <li>
    <strong>Back-end:</strong>
    A camada lógica do sistema, responsável pelo processamento de regras de negócio
    e comunicação com o servidor.
  </li>
  <li>
    <strong>Banco de Dados:</strong>
    O local onde as informações, como cadastros e registros, são armazenadas e organizadas.
  </li>
</ul>

<h3>Design e Experiência do Usuário (UX/UI)</h3>

<p>
  Antes do desenvolvimento do front-end, aplicam-se conceitos de design para
  garantir a eficácia da interface.
</p>

<ul>
  <li>
    <strong>User Experience (UX):</strong>
    Focado no comportamento e nas necessidades do usuário. Utiliza pesquisas e testes
    para garantir que a navegação seja fluida e satisfatória.
  </li>
  <li>
    <strong>User Interface (UI):</strong>
    Focado na estética e nos elementos interativos, como cores, botões e menus. Busca
    criar uma interface visualmente atraente e funcional.
  </li>
</ul>

<h3>Requisitos de uma Interface Moderna</h3>

<p>
  Uma interface de qualidade deve atender a critérios técnicos e sociais que
  impactam diretamente na retenção do usuário.
</p>

<ul>
  <li>
    <strong>Resposividade:</strong>
    Adaptação do layout para diferentes dispositivos (computadores, tablets e celulares).
  </li>
  <li>
    <strong>Acessibilidade e Inclusão:</strong>
    Design pensado para que pessoas com deficiências ou diferentes faixas etárias
    utilizem o sistema sem barreiras.
  </li>
  <li>
    <strong>Desempenho:</strong>
    Otimização de elementos para garantir um carregamento rápido das páginas.
  </li>
</ul>

<h3>Linguagens para Front-end</h3>

<h4>HTML (HyperText Markup Language)</h4>

<p>
  O HTML é uma <strong>linguagem de marcação</strong>, não de programação, pois
  carece de lógica (como loops ou condicionais). Sua função principal é
  estabelecer a <strong>estrutura e a organização</strong> do conteúdo da página.
</p>

<ul>
  <li>
    <strong>Elementos:</strong>
    Utiliza tags como &lt;h1&gt;, &lt;p&gt;, &lt;a&gt; e &lt;img&gt; para definir
    títulos, parágrafos, links e imagens.
  </li>
  <li>
    <strong>Interação Inicial:</strong>
    Permite a entrada de dados pelo usuário (formulários), possibilitando um nível
    básico de interação com o site.
  </li>
</ul>

<h4>CSS (Cascading Style Sheets)</h4>

<p>
  O CSS é a tecnologia responsável pela <strong
    >estilização e apresentação visual</strong
  > do conteúdo pelo HTML.
</p>

<ul>
  <li>
    <strong>Estética:</strong>
    Controla layouts, cores, fontes, margens e espaçamentos.
  </li>
  <li>
    <strong>Resposividade:</strong>
    Permite que as páginas de adaptem a diferentes tamanhos de tela.
  </li>
  <li>
    <strong>Dinamismo Visual:</strong>
    Suporta animações e transições para melhorar a experiência do usuário.
  </li>
  <li>
    <strong>Reutilização:</strong>
    Um único arquivo CSS pode ser aplicado a vários documentos HTML; ao alterar o
    estilo no arquivo central, todas as páginas vinculadas são atualizadas automaticamente.
  </li>
</ul>

<h4>JavaScript</h4>

<p>
  O JavaScript é uma <strong>linguagem de programação</strong> propriamente
  dita, interpretada pelo navegador, que adiciona
  <strong>interatividade e comportamento dinâmico</strong> às páginas.
</p>

<ul>
  <li>
    <strong>Atualização em tempo real:</strong>
    Permite modificar o conteúdo e a estrutura da página sem a necessidade de recarregá-la
    por completo.
  </li>
  <li>
    <strong>Assincronismo:</strong>
    Solicita e recebe dados do servidor em segundo plano, garantindo que a experiência
    do usuário não seja interrompida por novas requisições de carregamento.
  </li>
  <li>
    <strong>Características:</strong>
    É orientada a objetos e possui sintaxe similar à linguagem Java, focando na criação
    de aplicações web fluidas.
  </li>
</ul>

<h3>Responsabilidades do Back-end</h3>

<p>
  O back-end garante que a aplicação funcione corretamente, fornecendo a lógica
  necessária para o front-end. Suas funções principais incluem:
</p>

<ul>
  <li>
    <strong>Gerenciamento de Dados:</strong>
    Armazenamento e manipulação de informações.
  </li>
  <li>
    <strong>Lógica de Negócios</strong>
    Execução de regras complexas (ex: validação de saldo bancário ou transferências).
  </li>
  <li>
    <strong>Autenticação:</strong>
    Controle de acesso e segurança dos usuários.
  </li>
  <li>
    <strong>Comunicação:</strong>
    Exposição de APIs para integrar diferentes partes da aplicação ou serviços externos.
  </li>
  <li>
    <strong>Performance e Escalabilidade:</strong>
    Garantir respostas rápidas e suporte a múltiplos acessos simultâneos.
  </li>
</ul>

<h3>Componentes do Ecossistema Back-end</h3>

<h4>Linguagens de Programação</h4>

<ul>
  <li>
    <strong>PHP:</strong>
    Linguagem de script popular, simples e com forte integração ao HTML.
  </li>
  <li>
    <strong>Node.js:</strong>
    Permite utilizar JavaScript no lado do servidor, focando em alta performance.
  </li>
  <li>
    <strong>Python:</strong>
    Valorizada pela legibilidade, comumente usada com frameworks específicos.
  </li>
  <li>
    <strong>Ruby:</strong>
    Focada em produtividade e simplicidade de escrita.
  </li>
  <li>
    <strong>Java:</strong>
    Linguagem robusta e segura, padrão em grandes sistemas corporativos.
  </li>
</ul>

<h4>Servidores Web e Bancos de Dados</h4>

<ul>
  <li>
    <strong>Servidores:</strong>
    Responsáveis por processar as requisições, destacando-se o
    <strong>Apache</strong>
    (flexível), o <strong>Nginx</strong> (eficiente em conexões simultâneas) e o
    <strong>IIS</strong> (ambiente Windows).
  </li>
  <li>
    <strong>Bancos de Dados SQL:</strong>
    Relacionais (ex: MySQL, PostgreSQL) que utilizam lingugem estruturada para gerenciar
    dados.
  </li>
  <li>
    <strong>Bancos de Dados NoSQL:</strong>
    Não relacionais (ex: MongoDB), ideais para formatos de dados flexíveis e escaláveis.
  </li>
</ul>

<h4>APIs e Frameworks</h4>

<ul>
  <li>
    <strong>APIs:</strong>
    Definem as regras de comunicação. facilitando a troca de informações entre front-end
    e back-end.
  </li>
  <li>
    <strong>Frameworks:</strong>
    Ferramentas que aceleram o desenvolvimento e impõem padrões de organização, como
    <strong>Django</strong>
    (Python), <strong>Spring</strong> (Java),
    <strong>Express</strong> (Node.js) e <strong>Ruby on Rails</strong> (Ruby).
  </li>
</ul>

<h3>Configuração do Ambiente e Diretórios</h3>

<p>
  Para que o servidor local consiga processar o projeto, os arquivos devem ser
  armazenados em um local específico:
</p>

<ul>
  <li>
    <strong>Diretório Padrão:</strong>
    O projeto deve ser criado dentro da pasta C:\xampp\htdocs.
  </li>
  <li>
    <strong>Nomenclatura:</strong>
    É recomendável criar uma pasta específica para o projeto (ex: projeto_01) sem
    utilizar espaços ou caracteres especiais no nome.
  </li>
</ul>

<h3>utilizando o Visual Studio Code (VS Code)</h3>

<p>
  O VS Code é a ferramenta (IDE) utilizada para escrever e gerenciar o código:
</p>

<ul>
  <li>
    <strong>Abertura:</strong>
    Para iniciar, utiliza-se a opção File &gt; Open Folder para selecionar a pasta
    do projeto criada no diretório do Xampp.
  </li>
  <li>
    <strong>Criação de Arquivos:</strong>
    Novos arquivos são gerados dentro da interface, devendo receber a extensão correspondente
    à linguagem utilizada (.php, .css, etc).
  </li>
</ul>

<h3>Estrutura de Arquivos do Projeto</h3>

<p>
  A organização básica de um projeto que integra Front-end e Back-end segue este
  modelo:
</p>

<ul>
  <li>
    <strong>index.php:</strong>
    O arquivo principal localizado na raíz do projeto. Ele centraliza tanto o código
    <strong>PHP</strong>
    (lógica de servidor) quanto o <strong>HTML</strong> (estrutura da página).
  </li>
  <li>
    <strong>Pasta CSS:</strong>
    Uma subpasta criada para organizar os arquivos de estilo.
  </li>
  <li>
    <strong>style.css:</strong>
    Arquivo localizado dentro da pasta CSS, responsável por toda a parte visual e
    design da aplicação.
  </li>
</ul>

<h3>Estruturação do Código (CSS, HTML e PHP)</h3>

<p>
  A construção do projeto exige atenção rigorasa à <strong>sintaxe</strong>. A
  ausência de caracteres como pontos e vírgulas (;) ou chaves (&#123; &#125)
  impede o funcionamento do código.
</p>

<ul>
  <li>
    <strong>CSS (style.css):</strong> Contém as regras de design e identidade visual
    da página.
  </li>
  <li>
    <strong>Integração (index.php):</strong> O arquivo principal combina o
    <strong>HTML</strong>
    (estrutura do front-end) com o <strong>PHP</strong> (lógica do back-end). No
    exemplo citado, o PHP é utilizado de forma simples para exibir a data atual na
    página.
  </li>
  <li>
    <strong>Aprendizado Contínuo:</strong> O uso de plataformas como o W3Schools
    é recomendado para consultar tutoriais e aprofundar o conhecimento nas sintaxes
    dessas linguagens.
  </li>
</ul>

<h3>Execução com Servidor Local (XAMPP)</h3>

<p>
  Para visualizar a aplicação em funcionamento, é necessário simular um ambiente
  de servidor:
</p>

<ol>
  <li>
    <strong>Ativação:</strong> Abrir o painel de controle do
    <strong>XAMPP</strong> e iniciar (Start) os serviços necessários (como o Apache).
  </li>
  <li>
    <strong>Acesso via Navegador:</strong> Utilizar um navegador (ex: Chrome) e digitar
    o endereço na barra de URL.
  </li>
  <li>
    <strong>Sintaxe da URL:</strong> O padrão de acesso é localhost/nome_da_pasta_do_projeto.
    No exemplo, utiliza-se localhost/projeto_01.
  </li>
</ol>

<h4>Resultado Esperado</h4>

<p>
  Ao carregar a URL, o navegador processa o HTML e o CSS para exibir a interface
  visual, enquanto o servidor interpreta o código PHP para entregar os dados
  dinâmicos (como a data), resultando na página web executada localmente.
</p>

<h3>Conclusão: Fluxo do Desenvolvimento</h3>

<p>
  O processo de criação de uma aplicação web foi abordado desde a infraestrutura
  até a interface final, consolidando os seguintes pontos:
</p>

<ul>
  <li>
    <strong>Arquitetura e Comunicação:</strong> Compreensão de como as informações
    trafegam entre o usuário e o servidor.
  </li>
  <li>
    <strong>Pilares da Aplicação:</strong> Divisão clara entre
    <strong>Front-end</strong>
    (interface e experiência), <strong>Back-end</strong> (lógica e
    processamento) e <strong>Banco de Dados</strong> (armazenamento).
  </li>
  <li>
    <strong>Fase de Planejamento:</strong> Importância dos estudos de
    <strong>UX</strong>
    (Experiência do Usuário) e <strong>UI</strong> (Interface do Usuário) antes da
    escrita do código.
  </li>
</ul>

<h4>Integração Prática e Ferramentas</h4>

<p>
  A aplicação dos conceitos foi realizada através de ferramentas padrão do
  mercado para simular um ambiente real de desenvolvimento:
</p>

<ul>
  <li>
    <strong>IDE (Visual Studio Code):</strong> Utilizada para a escrita e organização
    dos arquivos do projeto.
  </li>
  <li>
    <strong>Linguagens Essenciais:</strong> Uso conjunto de
    <strong>HTML</strong>
    para estruturação,
    <strong>CSS</strong> para estilização e <strong>PHP</strong> para a lógica de
    servidor.
  </li>
  <li>
    <strong>Servidor Local (XAMPP):</strong> Ferramenta crucial para interpretar
    o código Back-end e disponibilizar a página para acesso via navegador (localhost).
  </li>
</ul>

<p>
  A prática demonstrou a "conversação" entre as camadas: o navegador solicita o
  arquivo, o servidor (XAMPP) processa a lógica em PHP, aplica as regras de
  estilo do CSS e entrega o conteúdo estruturado em HTML para o usuário final.
</p>
