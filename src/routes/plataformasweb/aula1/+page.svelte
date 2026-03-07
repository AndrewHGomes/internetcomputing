<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Introdução às Plataformas Web</h2>

<Audios modulo="M10" aulas={["01", "02", "03", "04"]} />

<p>
  A evolução da internet exigiu a criação de ferramentas que permitissem a
  usuários sem conhecimento profundo em programação desenvolverem suas próprias
  páginas. Com o tempo, as páginas simples tornaram-se aplicações complexas,
  consolidando o conceito de plataformas web como base fundamental para o
  desenvolvimento moderno
</p>

<p>
  Plataformas web são softwares que fornecem o suporte necessário para o
  desenvolvimento, hospedagem e manutenção de aplicações voltadas para a
  internet. Elas integram ferramentas, frameworks, serviços e bibliotecas,
  funcionando como um ecossistema que simplifica o trabalho do desenvolvedor na
  criação de sites e serviços online
</p>

<h3>Importância no Desenvolvimento</h3>

<p>
  A utilização dessas plataformas é justificada por pilares que otimizam a
  produção e a confiabilidade dos projetos:
</p>

<ul>
  <li>
    <strong>Facilidade de uso:</strong>
    Interfaces amigáveis que permitem ao desenvolvedor focar mais na funcionalidade
    e no design do que em códigos de infraestrutura.
  </li>
  <li>
    <strong>Rapidez no desenvolvimento:</strong>
    Uso de ferramentas e templates prontos que reduzem drasticamente o tempo entre
    a criação e o lançamento no mercado.
  </li>
  <li>
    <strong>Escalabilidade:</strong>
    Estruturas preparadas para suportar o crescimento do volume de usuários e de
    transações sem perda de desempenho.
  </li>
  <li>
    <strong>Segurança:</strong>
    Implementação de protocolos robustos para garantir a proteção de dados sensíveis
    e a integridade das comunicações.
  </li>
  <li>
    <strong>Manutenção e atualização:</strong>
    Facilidade em realizar correções e melhorias de forma contínua, garantindo que
    o serviço permaneça online durante as atualizações.
  </li>
</ul>

<h3>Plataformas Web e Frameworks</h3>

<p>
  A evolução das ferramentas web permitiu que a rede se expandisse para áreas
  como comércio, educação e redes sociais. Embora muitas páginas ainda foquem na
  integração humana direta, o desenvolvimento moderno se divide entre
  ferramentas para usuários comuns e estruturas avançadas para programadores.
</p>

<h4>Exemplos de Plataformas Web (No-Code/Low-Code)</h4>

<p>
  Estas plataformas são ideais para quem possui pouco ou nenhum conhecimento em
  programação, oferecendo interfaces visuais e hospedagem integrada:
</p>

<ul>
  <li>
    <strong>WordPress:</strong>
    Focado originalmente em blogs, oferece versões para hospedagem própria ou nos
    servidores da empresa.
  </li>
  <li>
    <strong>Wix:</strong>
    Utiliza o sistema de "arrastar e soltar", sendo dependente da sua própria infraestrutura
    de hospedagem.
  </li>
  <li>
    <strong>Shopify:</strong>
    Especializada em e-commerce, oferece um ambiente intuitivo e seguro para lojas
    online.
  </li>
  <li>
    <strong>Magento:</strong>
    Plataforma de código aberto para e-commerce, voltada para negócios que exigem
    alta personalização e controle total da operação.
  </li>
</ul>

<h4>Exemplos de Frameworks</h4>

<p>
  Frameworks são conjuntos de bibliotecas e ferramentas que fornecem uma
  estrutura base para desenvolvedores. Eles permitem o reuso de código e
  agilizam a criação de aplicações complexas.
</p>

<ul>
  <li>
    <strong>Django (Python):</strong>
    Framework de alto nível, robusto e seguro. É utilizado por grandes empresas como
    Instagram e YouTube devido à sua agilidade na criação de funcionalidades.
  </li>
  <li>
    <strong>Ruby on Rails (Ruby):</strong>
    Focado em produtividade, compartilha uma filosofia de design similar ao Django,
    facilitando o roteamento de URLs e o acesso a banco de dados.
  </li>
  <li>
    <strong>Express (Node.js/JavaScript):</strong>
    Leve e eficiente, facilita a transição de desenvolvedores do lado do cliente
    (front-end) para o servidor (back-end), embora dependa de bibliotecas externas
    para bancos de dados.
  </li>
  <li>
    <strong>Laravel (PHP):</strong>
    Oferece recursos avançados como roteamento rápido, processamento em segundo plano
    e uma sitaxe intuitiva para manipulação de dados (ORM).
  </li>
  <li>
    <strong>ASP.NET (C#/.NET):</strong>
    Framework de código aberto da Microsoft, desenvolvido para a criação de serviços
    e aplicações web modernas.
  </li>
</ul>

<h3>Componentes Básicos de uma Plataforma Web</h3>

<p>
  O desenvolvimento de sistemas para internet depende da integração de quatro
  componentes fundamentais que trabalham em conjunto para entregar a aplicação
  ao usuário.
</p>

<h4>Estrutura Técnica</h4>

<ul>
  <li>
    <strong>Servidores Web:</strong>
    São computadores especializados que armazenam e hospedam os sites e aplicações.
    Sua função é processar os pedidos e entregar os arquivos ao navegador do cliente
    quando solicitados.
  </li>
  <li>
    <strong>Bancos de Dados:</strong>
    É o sistema responsável pelo armazenamento persistente de informações. Ele guarda
    dados essenciais, como cadastros de usuários e históricos de compras, permitindo
    que essas informações sejam recuperadas em acessos futuros.
  </li>
  <li>
    <strong>Front-end:</strong>
    Compreende toda a interface visual e a parte interativa da aplicação. É o que
    o usuário vê e com o que interage, incluindo o design, o layout das telas e o
    comportamento dos botões e menus.
  </li>
  <li>
    <strong>Back-end:</strong>
    É o "cérebro" da aplicação, responsável pela lógica de programação, segurança
    e comunicação com o banco de dados. Ele opera nos bastidores, garantindo que
    o processamento das regras de negócio funcione corretamente.
  </li>
</ul>

<h4>Fluxo de uma Requisição Web</h4>

<p>
  O funcionamento de uma aplicação web baseia-se no ciclo de <strong
    >Requisição e Resposta</strong
  >:
</p>

<ol>
  <li>O <strong>cliente</strong> digita uma URL no navegador;</li>
  <li>
    O navegador localiza o endereço <strong>IP do servidor</strong> correspondente
    ao domínio;
  </li>
  <li>Uma conexão é estabelecida e a <strong>requisição</strong> é enviada;</li>
  <li>
    O <strong>servidor processa</strong> o pedido (podendo consultar o Back-end e
    o Banco de Dados);
  </li>
  <li>
    O servidor envia uma <strong>resposta</strong> de volta, que o navegador traduz
    na página visual que o usuário acessa.
  </li>
</ol>

<h3>Arquitetura Web: Fundamentos e Modelos</h3>

<p>
  A arquitetura web define a estrutura e organização dos componentes de uma
  aplicação. Sua escolha impacta diretamente o desempenho, a segurança, a
  manutenção e a <strong>escalabilidade</strong>, que é a capacidade do sistema
  se adaptar ao aumento da carga de trabalho sem perder eficiência.
</p>

<h4>Arquitetura Cliente-Servidor</h4>

<p>
  É o modelo mas básico, onde as funções são divididas entre quem solicita e
  quem atende. O
  <strong>cliente</strong> (navegador ou aplicativo) faz uma requisição, e o
  <strong>servidor</strong> (software ou hardware) fornece o serviço ou dado solicitado.
</p>

<ul>
  <li>
    <strong>Vantagens:</strong>
    Implementação simples e manutenção facilitada pelo servidor centralizado.
  </li>
  <li>
    <strong>Desvantagens:</strong>
    Ponto único de falha; se o servidor cair, todo o sistema fica indisponível para
    todos os usuários.
  </li>
</ul>

<h4>Arquitetura Multicamadas</h4>

<p>
  Neste modelo, a aplicação é fragmentada em camadas especializadas que
  trabalham de forma sequencial. O fluxo segue da interface para o processamento
  e, então, para o armazenamento.
</p>

<ul>
  <li>
    <strong>Camada de Apresentação (Front-end):</strong>
    Interface de integração com o usuário.
  </li>
  <li>
    <strong>Camada de Lógica de Negócios (Back-end):</strong>
    Processamento de dados e regras da aplicação.
  </li>
  <li>
    <strong>Camada de Dados:</strong>
    Local de armazenamento (Banco de Dados).
  </li>
  <li>
    <strong>Vantagens:</strong>
    Alta escalabilidade e facilidade de manutenção, pois as camadas são independentes.
  </li>
  <li>
    <strong>Desvantagens:</strong>
    Custo de implementação mais elevado em comparação ao modelo simples.
  </li>
</ul>

<h4>Arquitetura de Microsserviços</h4>

<p>
  A aplicação é decomposta em pequenos serviços independentes e distribuídos,
  cada um focado em uma tarefa específica. A comunicação entre eles ocorre via
  APIs. O fluxo é gerenciado por um <strong>API Gateway</strong>, que recebe a
  requisição do usuário e a direciona para os serviços correspondentes.
</p>

<ul>
  <li>
    <strong>Vantagens:</strong>
    Maior resiliência (uma falha em um serviço não derruba o sistema todo) e autonomia
    para desenvolver e implantar cada parte separadamente.
  </li>
  <li>
    <strong>Desvantagens:</strong>
    Alta complexidade na gestão e na comunicação entre diversos serviços.
  </li>
</ul>

<h3>A Web e sua Estrutura</h3>

<p>
  A <strong>World Wide Web (WWW)</strong>, ou simplesmente Web, é um sistema de
  documentos interconectados acessados via internet através de navegadores. É
  importante distinguir que a Web e a Internet são conceitos diferentes, embora
  complementares: a <strong>Internet</strong>
  é a infraestrutura global de redes e servidores, enquanto a
  <strong>Web</strong> é o subconjunto de informações (páginas e conteúdos) que trafega
  sobre essa infraestrutura.
</p>

<h4>Componentes Principais da Web</h4>

<p>
  Para que a Web funcione, ela depende de uma estrutura composta por quatro
  pilares fundamentais:
</p>

<ul>
  <li>
    <strong>Páginas Web:</strong>
    São documentos digitais acessíveis através de um endereço específico, a URL (como
    blogs e sites de notícias).
  </li>
  <li>
    <strong>Navegadores (Browsers):</strong>
    São os softwares que permitem ao usuário visualizar e interagir com as páginas
    web. Exemplos comuns incluem Google Chrome, Microsoft Edge, Mozilla Firefox e
    Safari.
  </li>
  <li>
    <strong>Servidores Web:</strong>
    São os computadores (hardware) e sistemas (software) responsáveis por armazenar
    e "hospedar" os sites, enviando-os aos navegadores quando solicitados.
  </li>
  <li>
    <strong>Protocolos de Comunicação:</strong>
    São as regras e padrões que permitem a troca de informações entre os diferentes
    componentes da rede.
  </li>
</ul>

<h3>Conclusão: Facilitadores de Desenvolvimento e Fluxo da Web</h3>

<p>
  O crescimento da internet impulsionou ferramentas que simplficaram a criação
  de sites. Existem <strong>plataformas web</strong> voltadas para usuários sem
  conhecimento técnico, permitindo a construção de páginas de forma visual. Para
  os desenvolvedores, o trabalho é otimizado pelo uso de
  <strong>frameworks</strong>, que oferecem bibliotecas de códigos
  reaproveitáveis, agilizando a estruturação de aplicações complexas.
</p>

<p>
  O funcionamento da web baseia-se no ciclo de interação: o usuário utiliza uma
  interface para enviar uma solicitação que é processada pelo servidor, gerando
  uma resposta. Esse fluxo é organizado por diferentes modelos de <strong
    >arquitetura web</strong
  >, cada um com vantagens e desvantagens específicas em termos de custo,
  manutenção e disponibilidade.
</p>

<p>
  A infraestrutura de <strong>rede</strong> é o elemento que mantém clientes e servidores
  conectados. Ela viabiliza a comunicação e o compartilhamento de dados, sendo sustentada
  por diferentes estruturas de redes e servidores que garantem a conectividade global.
</p>
