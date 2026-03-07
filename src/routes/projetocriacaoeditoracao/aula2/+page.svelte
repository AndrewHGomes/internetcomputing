<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Introdução ao GIMP e sua Interface</h2>

<Audios modulo="M5" aulas={["05", "06", "07", "08"]} />

<p>
  O <strong>GIMP (GNU Image Manipulation Program)</strong> é um software gratuito
  e de código aberto voltado para a edição e criação de imagens. É uma alternativa
  acessível a softwares pagos, permitindo desde ajustes fotográficos simples até
  composições complexas. A instalação é realizada diretamente pelo site oficial ou
  pela Microsoft Store.
</p>

<h3>Estrutura do Software</h3>

<p>
  A interface do GIMP é modular, organizada para facilitar o acesso às funções
  de edição. Ao abrir o programa, o usuário encontra:
</p>

<ul>
  <li>
    <strong>Caixa de Ferramentas (Esquerda):</strong> Contém os ícones das ferramentas
    de edição (pincéis, seleção, borrachas, etc.).
  </li>
  <li>
    <strong>Opções de Ferramentas (Abaixo da Caixa):</strong> Exibe as configurações
    específicas da ferramenta selecionada (tamanho, opacidade, dureza).
  </li>
  <li>
    <strong>Janelas de Encaixe (Direita):</strong> Onde ficam as camadas, canais
    e pincéis.
  </li>
  <li>
    <strong>Área Central:</strong> Espaço onde a imagem será exibida e manipulada.
  </li>
</ul>

<h4>Funções dos Menus Principais</h4>

<p>
  Para trabalhar com uma imagem, utiliza-se o menu <strong
    >Arquivo &gt; Abrir</strong
  >. Com uma imagem ativa, os menus oferecem as seguintes funções:
</p>

<ul>
  <li>
    <strong>Arquivo:</strong> Gerenciamento de arquivos (salvar, exportar, imprimir).
  </li>
  <li>
    <strong>Editar:</strong> Comandos de copiar e colar, além das preferências do
    sistema.
  </li>
  <li>
    <strong>Selecionar:</strong> Ferramentas para isolar partes da imagem para edição.
  </li>
  <li>
    <strong>Imagem:</strong> Ajustes globais, como alteração de tamanho, resolução
    e modo de cor.
  </li>
  <li>
    <strong>Camada:</strong> Organização da composição em "folhas" sobrepostas, permitindo
    editar elementos de forma independente.
  </li>
  <li>
    <strong>Cores:</strong> Ajustes específicos de tonalidade, saturação, brilho
    e balanço de cores.
  </li>
  <li>
    <strong>Filtros:</strong> Aplicação de efeitos especiais, como desfoque, nitidez
    e distorções.
  </li>
  <li>
    <strong>Janelas:</strong> Gerencia a exibição das caixas de ferramentas e painéis
    laterais.
  </li>
</ul>

<h3>Ferramentas e Técnicas de Seleção</h3>

<p>
  A seleção é uma das tarefas mais frequentes na edição de imagens. Ela permite
  isolar elementos ou áreas específicas para que as alterações não afetem o
  restante da fotografia. No GIMP, as ferramentas de seleção estão agrupadas em
  ícones na barra de ferramentas; ao manter o mouse pressionado sobre um ícone,
  as variações daquela categoria são exibidas.
</p>

<h4>Tipos de Ferramentas de Seleção</h4>

<ul>
  <li>
    <strong>Retangular ou Elíptica:</strong> Para selecionar formas geométricas básicas.
  </li>
  <li>
    <strong>Seleção Livre (Laço):</strong> Permite desenhar o contorno manualmente
    ao redor do objeto desejado.
  </li>
  <li>
    <strong>Tesoura ou de Frente:</strong> Ferramentas inteligentes que auxiliam
    no contorno de objetos complexos.
  </li>
  <li>
    <strong>Seleção Contígua (Varinha Mágica) ou por Cor:</strong> Selecionam áreas
    com base na similaridade de cores; a ferramenta por cor seleciona todos os pixels
    daquela tonalidade em qualquer parte da imagem.
  </li>
</ul>

<h4>Manipulação e Inversão</h4>

<p>
  Após realizar uma seleção, o usuário ganha controle total sobre a área
  isolada, podendo alterar cores, aplicar filtros ou excluir o conteúdo sem
  atingir as áreas não selecionadas.
</p>

<p>
  Um recurso essencial é a <strong>Inversão de Seleção</strong> (menu Selecionar
  &gt; Inverter). Esta função troca o que está selecionado pelo que não está. Por
  exemplo, ao selecionar um objeto central e inverter a seleção, o usuário passa
  a controlar apenas o fundo da imagem. Isso facilita efeitos como manter um objeto
  colorido enquanto o restante da foto é transformado em preto e branco.
</p>

<h3>Manipulação de Imagem e Ajustes de Cores</h3>

<p>
  O menu <strong>Imagem</strong> e o menu <strong>Cores</strong> são os pilares para
  transformações globais em uma fotografia. Enquanto o primeiro foca na estrutura
  física e orientação da foto, o segundo trata da estética, iluminação e fidelidade
  cromática.
</p>

<h4>Transformações Estruturais (Menu Imagem)</h4>

<p>
  Este menu permite alterar as propriedades físicas da imagem como um todo. As
  funções mais comuns incluem:
</p>

<ul>
  <li>
    <strong>Cortar:</strong> Redimensionar a área visível, removendo bordas ou focando
    em um detalhe.
  </li>
  <li>
    <strong>Girar:</strong> Alterar o ângulo da foto (90°, 180° ou ângulos personalizados).
  </li>
  <li>
    <strong>Inverter:</strong> Espelhar a imagem horizontal ou verticalmente.
  </li>
</ul>

<h4>Ajustes Estéticos e Corretivos (Menu Cores)</h4>

<p>
  O menu Cores é utilizado para manipular a atmosfera da fotografia e corrigir
  falhas de captura.
</p>

<ul>
  <li>
    <strong>Temperatura:</strong> Ajusta o equilíbrio entre tons quentes (alaranjados)
    e frios (azulados).
  </li>
  <li>
    <strong>Matiz-Croma:</strong> Permite alterar radicalmente as cores da imagem
    (ex: transformar tons azuis em verdes).
  </li>
  <li>
    <strong>Atributos Básicos:</strong> Controle de brilho, contraste, saturação
    (intensidade da cor) e exposição (quantidade de luz).
  </li>
</ul>

<h4>Calibragem de Níveis</h4>

<p>
  A calibração é essencial para fotos que não possuem um bom equilíbrio de luz
  original. Através do caminho <strong>Cores &gt; Níveis</strong>, é possível
  equalizar a imagem utilizando os conta-gotas de ponto preto e ponto branco:
</p>

<ol>
  <li>
    Seleciona-se o ícone do ponto escuro e clica-se na área mais preta da foto.
  </li>
  <li>
    Seleciona-se o ícone do ponto claro e clica-se na área mais branca da foto.
    Este processo define os limites de contraste, tornando a imagem mais
    impactante e equilibrada.
  </li>
</ol>

<h3>Camadas e Composições</h3>

<p>
  As <strong>camadas</strong> são o fundamento das montagens fotográficas, permitindo
  trabalhar com múltiplos elementos simultaneamente sem que um interfira permanentemente
  no outro. No GIMP, cada vez que você copia um elemento de uma imagem e o cola em
  outra, uma nova camada é criada, funcionando como uma película transparente sobreposta
  à base original. A manipulação de camadas permite criar cenários inexistentes na
  realidade, unindo elementos de diferentes contextos em uma única composição.
</p>

<h4>Fluxo de Trabalho com Camadas</h4>

<ul>
  <li>
    <strong>Criação:</strong> O processo básico consiste em selecionar um objeto
    de uma foto, copiá-lo e colá-lo sobre outra imagem.
  </li>
  <li>
    <strong>Independência:</strong> Cada camada pode ser editada, colorida ou movida
    de forma isolada, sem alterar o fundo ou as outras camadas.
  </li>
  <li>
    <strong>Redimensionamento:</strong> Para ajustar o tamanho do elemento
    colado ao novo cenário, utiliza-se o caminho
    <strong>Camada &gt; Transformação.</strong>
  </li>
  <li>
    <strong>Posicionamento:</strong> A ferramenta de movimento é usada para colocar
    o objeto no local exato da composição.
  </li>
  <li>
    <strong>Gerenciamento:</strong> É fundamental monitorar a janela de
    <strong>Camadas</strong> (no lado direito da tela) para garantir que você está
    trabalhando na camada correta e para organizar a ordem de sobreposição dos elementos.
  </li>
</ul>

<h3>Filtros no GIMP</h3>

<p>
  Os filtros são recursos utilizados para aplicar efeitos visuais automáticos em
  fotografias, técnica que existe muito antes das redes sociais. No GIMP, eles
  estão organizados por categorias dentro do menu <strong>Filtros</strong>.
  Esses efeitos podem ser aplicados em toda a fotografia ou apenas em uma área
  previamente isolada por uma ferramenta de seleção.
</p>

<p>
  A aplicação de um filtro permite transformar o estilo de uma imagem de forma
  instantânea, alterando sua textura, iluminação ou estrutura. Como as
  possibilidades são vastas, a experimentação direta em imagens de teste é a
  estratégia mais eficiente para compreender o resultado de cada opção.
</p>

<h4>Categorias e Exemplos de Filtros</h4>

<ul>
  <li>
    <strong>Artísticos:</strong> Transformam a fotografia em estilos de arte tradicional,
    como o efeito de Aquarela, que simula pinturas manuais.
  </li>
  <li>
    <strong>Distorções:</strong> Alteram a geometria ou a textura da imagem, como
    o efeito de Gravura, que cria ranhuras e padrões típicos de impressões antigas.
  </li>
  <li>
    <strong>Aplicação Seletiva:</strong> Se uma parte da imagem estiver selecionada,
    o filtro afetará apenas aquela região, permitindo efeitos localizados e composições
    criativas.
  </li>
</ul>

<h3>Conclusão</h3>

<p>
  O primeiro contato com o <strong>GIMP</strong> revela uma ferramenta poderosa
  e versátil para a criação e edição de imagens. Sua principal vantagem
  competitiva, além das funcionalidades técnicas, é ser um
  <strong>software gratuito e de código aberto</strong>. Isso permite o uso
  profissional em qualquer contexto — seja em empresas ou em projetos autônomos
  — sem custos de licenciamento. A eficiência no uso do software não depende
  apenas da teoria, mas da experiência prática acumulada.
</p>

<h4>Diretrizes para o Aprendizado</h4>

<ul>
  <li>
    <strong>Prática Constante:</strong> A maestria na ferramenta é alcançada através
    do uso contínuo. Quanto mais tempo dedicado à manipulação de imagens, mais intuitivo
    se torna o fluxo de trabalho.
  </li>
  <li>
    <strong>Exploração Livre:</strong> O processo de "fuçar" — testar filtros, ajustar
    cores e experimentar seleções — é a forma mais rápida de descobrir o potencial
    de cada recurso.
  </li>
  <li>
    <strong>Agilidade no Desenvolvimento:</strong> A familiaridade com a interface
    e os menus resulta em um trabalho mais ágil e profissional, reduzindo o tempo
    de execução de projetos complexos.
  </li>
</ul>
