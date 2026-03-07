<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Introdução ao Desenvolvimento Mobile</h2>

<Audios modulo="M9" aulas={["01", "02", "03", "04"]} />

<p>
  O crescimento do setor é impulsionado pela Indústria 4.0 e pela necessidade de
  múltiplos canais de acesso. Atualmente, a fronteira entre o desenvolvimento
  <strong>mobile</strong> e <strong>web</strong> é tênue, com muitas tecnologias
  sendo compartilhadas entre ambas as plataformas.
</p>

<h3>Modelos de Desenvolvimento</h3>

<p>
  Existem três abordagens principais para a criação de aplicativos, cada uma com
  características de distribuição e execução distintas:
</p>

<ul>
  <li>
    <strong>Nativo:</strong> Desenvolvido especificamente para um sistema operacional
    (Android ou iOS), utilizando as linguagens originais da plataforma.
  </li>
  <li>
    <strong>Híbrido:</strong> Desenvolvido com linguagens web, mas empacotado como
    um aplicativo para ser distribuído em lojas (App Store/Play Store).
  </li>
  <li>
    <strong>Web:</strong> Sites otimizados para execução exclusiva dentro de navegadores
    móveis, sem possibilidade de empacotamento ou distribuição em lojas.
  </li>
</ul>

<h4>Comparativo: Nativo vs. Híbrido</h4>

<p>
  A escolha entre as vertentes depende do equilíbrio entre custo, tempo e
  performance.
</p>

<ul>
  <li>
    <strong>Desenvolvimento Nativo:</strong> Oferece o melhor desempenho e acesso
    total ao hardware, porém exige um desenvolvimento separado para cada plataforma,
    aumentando o custo e o tempo.
  </li>
  <li>
    <strong>Desenvolvimento Híbrido:</strong> Permite o reaproveitamento de código
    em vários sistemas e possui desenvolvimento mais ágil. No entanto, apresenta
    desempenho inferior devido às camadas extras de tradução entre o código e o hardware.
  </li>
</ul>

<h3>Vantagens e Desvantagens do Modelo Híbrido</h3>

<h4>Vantagens:</h4>

<ul>
  <li>
    <strong>Migração facilitada:</strong> Única base de código para diferentes sistemas
    operacionais.
  </li>
  <li>
    <strong>Custo reduzido:</strong> Geralmente mais barato que o desenvolvimento
    de múltiplos apps nativos.
  </li>
  <li>
    <strong>Manutenção simplificada:</strong> Atualizações não exigem a recriação
    total do aplicativo.
  </li>
  <li>
    <strong>Acesso a recursos:</strong> Utiliza plugins para acessar hardware como
    câmera e GPS.
  </li>
</ul>

<h4>Desvantagens:</h4>

<ul>
  <li>
    <strong>Performance:</strong> Desempenho inferior ao nativo, perceptível em tarefas
    complexas.
  </li>
  <li>
    <strong>Design e Usabilidade:</strong> Limitações na criação de interfaces e
    experiência do usuário, pois tenta padronizar elementos para sistemas diferentes
    (Android e iOS).
  </li>
  <li>
    <strong>Limitação de execução:</strong> Geralmente depende de o app estar em
    primeiro plano e online para funcionar plenamente.
  </li>
</ul>

<h3>Infraestrutura de Desenvolvimento</h3>

<p>
  Para criar aplicativos, é necessário preparar o ambiente com ferramentas
  específicas, dependendo da abordagem escolhida:
</p>

<ul>
  <li>
    <strong>Desenvolvimento Nativo (Android):</strong> Exige a instalação do
    <strong> Android Studio </strong>. É uma plataforma robusta, porém pesada,
    recomendando-se o uso de pelo menos 8 GB de RAM.
  </li>
  <li>
    <strong>Desenvolvimento Híbrido:</strong> Utiliza editores mais leves, como
    o
    <strong>VS Code</strong> (código aberto e gratuito).
  </li>
  <li>
    <strong>Comum a ambos:</strong> É necessária a instalação do
    <strong>Android SDK</strong> (kit de desenvolvimento) para permitir o acesso
    às funcionalidades do sistema e o empacotamento do aplicativo.
  </li>
</ul>

<h4>O Trio Fundamental: HTML, CSS e JavaScript</h4>

<p>
  No contexto mobile (especialmente híbrido), o desenvolvimento utiliza as
  mesmas bases da web.
</p>

<ul>
  <li>
    <strong>HTML (Marcação):</strong> Funciona como um arquivo de texto
    estruturado. Utiliza <strong>tags</strong> para definir os elementos da página.
    Para testar, basta salvar um arquivo com a extensão .html e abri-lo em um navegador.
  </li>
  <li>
    <strong>CSS (Estilo):</strong> É a tecnologia responsável por
    <strong>formatar</strong> o código HTML, definindo cores, fontes, tamanhos e
    o layout visual do aplicativo.
  </li>
  <li>
    <strong>JavaScript (Lógica):</strong> Responsável por criar as funções e a interatividade
    do projeto.
  </li>
</ul>

<h4>Ferramentas e Referências</h4>

<ul>
  <li>
    <strong>Editores:</strong> Pode-se usar qualquer editor de texto sem formatação,
    sendo os editores de código (como VS Code) os mais adequados para organizar o
    trabalho.
  </li>
  <li>
    <strong>Aprendizado:</strong> O site <strong>W3Schools</strong> é citado como
    a principal referência prática, permitindo testar códigos de HTML, CSS e JS diretamente
    no navegador sem a necessidade de instalações complexas no início.
  </li>
</ul>

<h3>JavaScript e sua Versatilidade</h3>

<p>
  O JavaScript consolidou-se como uma das linguagens mais populares devido à sua
  onipresença na web e sua capacidade de lidar com elementos dinâmicos.
</p>

<ul>
  <li>
    <strong>Front-end:</strong> É o núcleo da interatividade em páginas e aplicativos,
    permitindo criar mapas, formulários inteligentes, cálculos e animações.
  </li>
  <li>
    <strong>Back-end:</strong> Com o surgimento do <strong>Node.js</strong>, o
    JavaScript expandiu-se para o lado do servidor, permitindo que um
    programador desenvolva todo o projeto (frente e fundo) usando uma única
    linguagem.
  </li>
  <li>
    <strong>Funcionalidade:</strong> No contexto mobile, é o JavaScript que dá "vida"
    ao sistema, conectando dados e implementando a lógica das funcionalidades.
  </li>
</ul>

<h3>Por que focar no Desenvolvimento Híbrido?</h3>

<p>
  O uso de tecnologias web (HTML, CSS e JS) para criar aplicativos móveis
  oferece vantagens estratégicas, especialmente para novos projetos e
  protótipos:
</p>

<ul>
  <li>
    <strong>Curva de Aprendizado:</strong> Exige menos conhecimento técnico específico
    de hardware, aproveitando o conhecimento de desenvolvimento web já existente.
  </li>
  <li>
    <strong>Flexibilidade:</strong> Permite atender às principais plataformas do
    mercado (Android e iOS) utilizando um único código-fonte.
  </li>
  <li>
    <strong>Manutenção e Custo:</strong> Facilita a disponibilização de atualizações
    e reduz drasticamente o custo de desenvolvimento em comparação ao modelo nativo.
  </li>
  <li>
    <strong>Agilidade:</strong> O uso de <strong>frameworks</strong> acelera o fluxo
    de trabalho, permitindo transformar ideias em aplicativos funcionais rapidamente.
  </li>
</ul>

<h3>Conclusão</h3>

<p>
  O foco principal deste estágio é a compreensão dos conceitos e da lógica por
  trás das tecnologias. A união entre a estrutura (HTML), a estética (CSS) e o
  comportamento (JavaScript) forma a base para a criação de aplicativos modernos
  e eficientes.
</p>
