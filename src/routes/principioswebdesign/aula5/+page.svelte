<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Evolução do Web Design e Multitelas</h2>

<Audios modulo="M6" aulas={["17", "18", "19", "20"]} />

<p>
  Diferente da década de 1990, quando o conteúdo era planejado para resoluções
  fixas, o cenário atual exige flexibilidade. O usuário transita entre desktops,
  notebooks e dispositivos móveis, demandando que o web designer estruture
  ambientes com experiências de navegação e consumo de conteúdo similares em
  todas as plataformas.
</p>

<h3>Arquitetura da Informação (AI) Web</h3>

<p>
  A Arquitetura da Informação é a disciplina que organiza, categoriza e
  apresenta o conteúdo de forma a tornar a navegação intuitiva e eficiente. Ela
  combina arte e ciência para transformar dados complexos em estruturas claras,
  focando na usabilidade e na recuperação rápida da informação em sites,
  intranets e comunidades online. Além da estética, a AI garante a
  funcionalidade e impacta diretamente em outras áreas:
</p>

<ul>
  <li>
    <strong>SEO e Marketing Digital:</strong> Facilita a leitura dos bots de busca
    e melhora o ranqueamento ao otimizar a experiência do usuário.
  </li>
  <li>
    <strong>UX Design:</strong> Reforça a acessibilidade e a orientação do conteúdo
    com foco nas necessidades do usuário.
  </li>
  <li>
    <strong>Dialética entre Belo e Funcional:</strong> A AI não ignora a estética,
    mas equilibra a aparência visual com a utilidade prática do ambiente digital.
  </li>
</ul>

<h4>Os 8 Princípios da AI (Dan Brown)</h4>

<p>
  Para guiar a criação de estruturas informacionais, utilizam-se oito
  fundamentos principais:
</p>

<ul>
  <li>
    <strong>Princípio dos Objetos:</strong> Trata o conteúdo como um organismo vivo,
    com ciclo de vida e comportamentos que exigem evolução constante.
  </li>
  <li>
    <strong>Princípio da Categorização:</strong> Agrupa conteúdos por similaridade
    e define seus atributos para facilitar a localização.
  </li>
  <li>
    <strong>Princípio da Divulgação:</strong> Gerencia a exibição de informações
    para manter o interesse do usuário sem sobrecarregá-lo.
  </li>
  <li>
    <strong>Princípio do Contexto:</strong> Considera o ambiente, a cultura e o comportamento
    do usuário para moldar o projeto.
  </li>
  <li>
    <strong>Princípio da Antecipação:</strong> Preve as necessidades e desejos do
    usuário, oferecendo opções antes mesmo de serem solicitadas.
  </li>
  <li>
    <strong>Princípio da Escaneabilidade:</strong> Estrutura o conteúdo para que
    seja lido e compreendido rapidamente através de uma visualização rápida.
  </li>
  <li>
    <strong>Princípio da Consistência:</strong> Mantém padrões visuais e funcionais
    para criar familiaridade e confiança na navegação.
  </li>
  <li>
    <strong>Princípio do Contraste:</strong> Utiliza a diferenciação visual para
    destacar itens prioritários e estabelecer uma hierarquia clara.
  </li>
</ul>

<h3>Sites Responsivos</h3>

<p>
  O conceito de site responsivo surgiu como resposta à transição dos acessos
  fixos (Desktops) para a diversidade de dispositivos móveis. Um site responsivo
  é projetado para se adequar automaticamente a diferentes tamanhos de tela e
  resoluções, garantindo que o conteúdo seja exibido de forma otimizada sem a
  necessidade de barras de rolagem horizontais ou conteúdos cortados. A
  implementação de um projeto responsivo baseia-se em uma tríade fundamental:
</p>

<h4>Layout Fluído (Grids Flexíveis)</h4>

<p>
  Diferente do design tradicional que utiliza medidas fixas (como Pixels ou
  Pontos), o layout fluído utiliza <strong>medidas relativas</strong>, como
  percentuais. Isso permite que a estrutura da página se comporte como uma
  proporção da área disponível, adaptando-se "naturalmente" ao espaço da tela em
  vez de ficar engessada em dimensões estáticas.
</p>

<h4>Imagens Flexíveis</h4>

<p>
  Seguindo a lógica do layout fluído, as imagens não possuem largura e altura
  fixas. Elas são configuradas para serem redimensionadas pelo navegador de
  acordo com a proporção da área onde estão inseridas, evitando que ultrapassem
  os limites da tela do dispositivo.
</p>

<h4>Media Queries (CSS)</h4>

<p>
  As Media Queries são expressões condicionais no código CSS que detectam as
  características do dispositivo do usuário, como a largura da tela. Elas
  permitem que o web designer defina regras de estilo específicas para
  diferentes intervalos de resolução, reorganizando o layout de forma
  inteligente para oferecer a melhor experiência em cada cenário (celular,
  tablet ou monitor).
</p>

<h3>Mobile First</h3>

<p>
  O conceito de <strong>Mobile First (Móvel Primeiro)</strong> estabelece que o planejamento
  e o desenvolvimento de um projeto digital devem começar pela versão voltada para
  dispositivos móveis, para só depois serem expandidos para telas maiores. Essa abordagem
  inverte a lógica tradicional devido à centralidade dos smartphones no acesso à
  internet e à necessidade de lidar primeiro com as maiores restrições de espaço
  e performance.
</p>

<h4>Diferença entre Responsivo e Mobile First</h4>

<p>Embora relacionados, não são sinônimos:</p>

<ul>
  <li>
    <strong>Design Responsivo:</strong> Foca em adaptar um site já existente para
    diferentes formatos de tela.
  </li>
  <li>
    <strong>Mobile First:</strong> É uma estratégia de design onde o foco inicial
    é a experiência no celular, tratando o desktop como uma expansão desta base.
  </li>
</ul>

<h4>Vantagens da Abordagem</h4>

<ul>
  <li>
    <strong>Inclusão Digital:</strong> Atende à maioria dos usuários que possuem
    apenas smartphones para acesso.
  </li>
  <li>
    <strong>Foco no Essencial:</strong> Força a priorização de conteúdos e funcionalidades
    devido ao espaço reduzido.
  </li>
  <li>
    <strong>Uso de Sensores:</strong> Permite aproveitar recursos nativos dos celulares,
    como geolocalização e notificações (push), para criar experiências contextuais.
  </li>
</ul>

<h4>Formas de Implementação</h4>

<p>
  Existem quatro maneiras principais de aplicar o conceito Mobile First em um
  projeto:
</p>

<ul>
  <li>
    <strong>Design Responsivo:</strong> Utiliza o mesmo código e medidas relativas
    para que o site se reajuste automaticamente a qualquer tela.
  </li>
  <li>
    <strong>Exibição Dinâmica:</strong> O servidor identifica o dispositivo do usuário
    e entrega um código HTML/CSS diferente para o mesmo endereço de site, permitindo
    personalização profunda.
  </li>
  <li>
    <strong>URLs Separados:</strong> Cria endereços distintos para cada versão (ex:
    www.site.com para desktop e m.site.com para mobile).
  </li>
  <li>
    <strong>Aplicativo (App):</strong> O conteúdo é desenvolvido dentro de um ambiente
    nativo do sistema operacional do celular, aproveitando ao máximo as configurações
    e alertas do aparelho.
  </li>
</ul>

<h3>Fundamentos do HTML – Estrutura</h3>

<p>
  O HTML (<strong>Hypertext Markup Language</strong>) é a linguagem de marcação
  padrão da web. Diferente das linguagens de programação, o HTML não possui
  lógica complexa ou processamento de dados; sua função é
  <strong>marcar, estruturar e organizar</strong> como o conteúdo (textos, imagens
  e links) será apresentado no navegador. A linguagem baseia-se em três pilares:
</p>

<ul>
  <li>
    <strong>Estrutura de Conteúdo:</strong> Define a hierarquia dos elementos.
  </li>
  <li>
    <strong>Tags:</strong> Sinais que delimitam as partes do texto e dão instruções
    ao navegador.
  </li>
  <li>
    <strong>Semântica:</strong> Atribui significado aos dados, permitindo que máquinas
    e motores de busca compreendam o conteúdo.
  </li>
</ul>

<h4>O Uso de Tags</h4>

<p>
  As tags funcionam como comandos de abertura e fechamento, indicadas pelos
  sinais &lt; &gt;.
</p>

<ul>
  <li><strong>Abertura:</strong> &lt;tag&gt; (ex: &lt;html&gt;)</li>
  <li><strong>Fechamento:</strong> &lt;/tag&gt; (ex: &lt;/html&gt;)</li>
</ul>

<p>
  O fechamento é obrigatório para indicar onde termina a instrução dada ao
  elemento, garantindo que a hierarquia do documento seja respeitada.
</p>

<h4>Estrutura Básica do Documento</h4>

<p>
  Uma página HTML segue uma organização lógica dividida em seções principais:
</p>

<ul>
  <li>
    <strong>HTML (&lt;html&gt;):</strong> É o elemento raiz que envolve todo o código
    da página, demarcando o início e o fim do documento.
  </li>
  <li>
    <strong>Head (&lt;head&gt;):</strong> A "cabeça" do documento. Contém os metadados
    (descrições, palavras-chave, autor, codificação). As informações aqui não aparecem
    visualmente para o usuário, mas são essenciais para o navegador e para o ranqueamento
    no Google (SEO).
  </li>
  <li>
    <strong>Body (&lt;body&gt;):</strong> O "corpo" da página. É a parte visível
    onde são inseridos todos os conteúdos de interação, como textos, títulos, imagens
    e vídeos.
  </li>
  <li>
    <strong>Footer (&lt;footer&gt;):</strong> O "rodapé". Espaço reservado para informações
    institucionais, direitos autorais, contatos e dados dos desenvolvedores.
  </li>
</ul>

<h3>Fundamentos do HTML – Atributos e Tags de Conteúdo</h3>

<p>
  Além das tags estruturais, o HTML utiliza tags específicas para organizar a
  hierarquia e os elementos internos do corpo da página (&lt;body&gt;). Elas
  definem a natureza de cada informação, como títulos, parágrafos e mídias.
</p>

<h4>Tags de Conteúdo Comuns</h4>

<ul>
  <li>
    <strong>Títulos (&lt;h1&gt; a &lt;h6&gt;):</strong> Estabelecem a hierarquia
    visual e de importância. O &lt;h1&gt; é o título principal (maior), enquanto
    o &lt;h6&gt; é o de menor nível.
  </li>
  <li>
    <strong>Parágrafos (&lt;p&gt;):</strong> Delimitam blocos de texto, evitando
    que o conteúdo se misture em um único bloco contínuo.
  </li>
  <li>
    <strong>Links (&lt;a&gt;):</strong> Utilizados para criar hiperligações entre
    páginas ou arquivos.
  </li>
  <li>
    <strong>Imagens (&lt;img&gt;):</strong> Tag utilizada para a inserção de elementos
    visuais.
  </li>
</ul>

<h4>Atributos: Especificando Elementos</h4>

<p>
  Os atributos são informações adicionais inseridas na <strong
    >tag de abertura</strong
  >
  que modificam o comportamento ou a aparência de um elemento. Eles funcionam em
  pares de <strong>nome="valor"</strong>. O uso de aspas (simples ou duplas) é
  necessário para definir o valor, recomendando-se manter a consistência em todo
  o código.
</p>

<h4>Principais Atributos e Exemplos</h4>

<ul>
  <li>
    <strong>style:</strong> Define estilos visuais diretamente no elemento, como
    cores e fontes.
    <ul>
      <li>
        <strong>Exemplo:</strong> &lt;h1 style="color: blue;"&gt; altera a cor do
        título para azul.
      </li>
    </ul>
  </li>
  <li>
    <strong>href (Hypertext Reference):</strong> Essencial para a tag de link
    (&lt;a&gt;), indica o destino ou a URL para onde o usuário será direcionado.
    <ul>
      <li><strong>Exemplo:</strong> &lt;a href="https://www.site.com"&gt;.</li>
    </ul>
  </li>
  <li>
    <strong>src (Source):</strong> Obrigatório para a tag de imagem
    (&lt;img&gt;), aponta o caminho (origem), o nome e o formato do arquivo de
    imagem.
    <ul>
      <li><strong>Exemplo:</strong> &lt;img src="foto.jpg"&gt;.</li>
    </ul>
  </li>
  <li>
    <strong>alt (Alternative Text):</strong> Fornece uma descrição textual da imagem
    para acessibilidade e motores de busca.
  </li>
</ul>

<h3>Conclusão: Essência da Arquitetura da Informação</h3>

<p>
  O conteúdo sintetiza os conceitos fundamentais da <strong>
    Arquitetura da Informação (AI)
  </strong>, reforçando que sua função principal é a transformação de dados
  complexos em estruturas navegáveis e acessíveis.
</p>

<h4>Essência da Arquitetura da Informação</h4>

<p>
  A AI atua como a ponte entre a organização técnica e a compreensão humana. Seu
  papel vai além da estética, focando na <strong
    >funcionalidade e praticidade</strong
  > dos ambientes digitais através de alguns pilares:
</p>

<ul>
  <li>
    <strong>Organização e Navegação:</strong> Foca em categorizar conteúdos para
    que a jornada do usuário seja intuitiva e eficiente.
  </li>
  <li>
    <strong>Valor Estratégico:</strong> Impacta diretamente o SEO e o Marketing Digital,
    pois uma estrutura clara facilita o mapeamento por motores de busca (como o Google).
  </li>
  <li>
    <strong>Princípios Operacionais:</strong> Utiliza estratégias como a
    <strong>categorização</strong>
    (agrupamento de itens semelhantes) e a <strong>antecipação</strong> (prever o
    que o usuário precisa antes mesmo de ele solicitar).
  </li>
  <li>
    <strong>Dialética do Design:</strong> Estabelece um equilíbrio onde a beleza
    visual (semiótica) deve obrigatoriamente caminhar junto à utilidade prática do
    site.
  </li>
</ul>
