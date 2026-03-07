<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Conceitos e Funções do Design</h2>

<Audios modulo="M4" aulas={["09", "10", "11", "12"]} />

<p>
  O design não deve ser confundido apenas com "desenho". Sua definição correta é
  <strong>projeto</strong>. Tudo o que é planejado para interagir com seres
  humanos — de uma caneta a um software — possui design. O papel do designer é
  projetar soluções intuitivas que facilitem a vida do usuário.
</p>

<p>
  Um conceito central é o de Affordance, que se refere à capacidade de um objeto
  (físico ou virtual) deixar claro sua utilidade à primeira vista. Um bom
  affordance fornece pistas imediatas de como operar algo, como um banco que
  sugere o ato de sentar ou uma maçaneta que indica o movimento de girar. Em
  interfaces complexas, como smartphones, o design precisa trabalhar mais para
  tornar essas funções compreensíveis. De acordo com a teoria de Löbach, um
  projeto perfeito deve equilibrar três funções básicas:
</p>

<ul>
  <li>
    <strong>Função Prática:</strong> O produto deve ser útil, funcional e facilitar
    a tarefa do usuário.
  </li>
  <li>
    <strong>Função Estética:</strong> O produto deve ser visualmente agradável e
    atraente para gerar engajamento.
  </li>
  <li>
    <strong>Função Simbólica:</strong> O produto deve transmitir significados e valores
    que vão além da sua aparência física.
  </li>
</ul>

<p>
  Para alcançar um design limpo e transmitir informações com clareza, a prática
  profissional se baseia em quatro princípios essenciais que serão detalhados a
  seguir: <strong>proximidade, alinhamento, repetição e contraste</strong>.
</p>

<h3>O Princípio da Proximidade</h3>

<p>
  O conceito de proximidade estabelece que itens relacionados entre si devem ser
  agrupados visualmente. Quando informações que compartilham o mesmo contexto
  são colocadas próximas, elas passam a ser percebidas como um grupo coeso, e
  não como elementos isolados e desconexos.
</p>

<p>
  A organização espacial serve para reduzir a desordem e facilitar a compreensão
  imediata do conteúdo. Agrupar elementos ajuda a organizar a informação na
  mente do usuário, tornando a leitura mais simples e intuitiva. Por outro lado,
  elementos que não possuem relação conceitual devem ser mantidos separados para
  evitar confusão. Exemplos práticos de aplicação:
</p>

<ul>
  <li>
    <strong>Cartões de visita:</strong> Separar o nome e o cargo do profissional
    das informações de contato (endereço e telefone) cria blocos de leitura distintos
    e claros.
  </li>
  <li>
    <strong>Listas de compras:</strong> Agrupar itens por categorias (alimentos,
    higiene, escritório) é mais eficiente do que listar produtos aleatoriamente.
  </li>
  <li>
    <strong>Interfaces digitais:</strong> Botões e menus que realizam funções semelhantes
    devem estar visualmente próximos para indicar que pertencem à mesma categoria
    de ação.
  </li>
</ul>

<h3>O Princípio do Alinhamento</h3>

<p>
  O <strong>alinhamento</strong> baseia-se na ideia de que nada deve ser posicionado
  de forma arbitrária em uma página ou tela. Cada elemento precisa estar visualmente
  conectado a outro, criando uma unidade coesa. Essa organização gera uma sensação
  de segurança e ordem para o cérebro, evitando que os itens pareçam meramente "jogados"
  no espaço.
</p>

<p>
  A aplicação correta do alinhamento utiliza "fios invisíveis" que ancoram os
  elementos entre si. Mesmo que os itens não estejam encostados nas margens, a
  relação de continuidade entre eles guia o olhar do usuário de forma fluida. O
  uso de alinhamentos bem definidos torna o design mais profissional e
  estruturado. Sobre as formas de alinhar, destacam-se os seguintes pontos:
</p>

<ul>
  <li>
    Alinhamento à Esquerda: É o padrão mais comum e seguro, facilitando a
    leitura e a ancoragem dos elementos.
  </li>
  <li>
    Alinhamento à Direita: Pode trazer sofisticação e modernidade, sendo uma
    alternativa interessante para atrair a atenção de forma diferenciada.
  </li>
  <li>
    Centralização: Embora não seja incorreta, é considerada comum e menos
    dinâmica. Deve ser evitada quando o objetivo é criar um layout mais elegante
    e marcante.
  </li>
  <li>
    Alinhamentos Compostos: É possível distribuir elementos em diferentes pontos
    (como um grupo à esquerda e outro à direita), desde que cada grupo mantenha
    sua própria coerência e conexão visual.
  </li>
</ul>

<h3>O Princípio da Repetição</h3>

<p>
  A <strong>repetição</strong> é o elemento que confere consistência e unidade ao
  design. Ao repetir certos aspectos visuais ao longo de um projeto, o designer cria
  um padrão que ajuda o usuário a se localizar e a prever a estrutura do conteúdo.
  Essa técnica gera conforto visual e profissionalismo, transformando elementos isolados
  em um conjunto coeso. A aplicação da repetição pode ser sutil ou marcante, utilizando
  diversos recursos:
</p>

<ul>
  <li>
    <strong>Tipografia:</strong> Usar o negrito consistentemente para destacar as
    informações mais importantes (como títulos ou nomes próprios).
  </li>
  <li>
    <strong>Elementos Gráficos:</strong> Utilizar linhas (fios), cores específicas
    ou formas geométricas de maneira recorrente para reforçar a identidade visual.
  </li>
  <li>
    <strong>Estrutura:</strong> Manter o mesmo layout para inícios de capítulos em
    um livro ou para cabeçalhos em um site.
  </li>
</ul>

<p>
  O objetivo principal é guiar o olhar do leitor. Ao padronizar o destaque das
  informações principais, o olho identifica primeiro o que é essencial e, em
  seguida, as informações secundárias. Como regra geral, a simplicidade na
  repetição é o que garante a sofisticação e a clareza do projeto.
</p>

<h3>O Princípio do Contraste</h3>

<p>
  O <strong>contraste</strong> ocorre quando dois elementos em um mesmo espaço
  são visualmente muito distintos entre si. A regra fundamental é a clareza: se
  dois itens não forem idênticos, eles devem ser
  <strong>muito diferentes</strong>. Diferenças sutis podem ser interpretadas
  como erro ou confusão visual, enquanto o contraste acentuado organiza a
  hierarquia e atrai a atenção. Para criar um contraste eficaz, o designer pode
  explorar diversos atributos:
</p>

<ul>
  <li>
    <strong>Tipografia:</strong> Combinar fontes com estilos opostos, como usar fontes
    com serifa para títulos e sem serifa para o corpo do texto.
  </li>
  <li>
    <strong>Cores:</strong> Utilizar tons contrastantes ou inversões (como o efeito
    negativo de preto e branco) para destacar seções específicas.
  </li>
  <li>
    <strong>Tamanho e Peso:</strong> Alternar entre elementos grandes e pequenos,
    ou traços finos e grossos, para indicar a importância de cada informação.
  </li>
</ul>

<p>
  O uso correto do contraste elimina a monotonia do layout e serve como um guia
  visual, deixando claro para o usuário onde ele deve focar primeiro.
</p>

<h3>Aplicação Integrada dos Princípios de Design</h3>

<p>
  A eficácia do design não reside no uso isolado de um princípio, mas na
  combinação estratégica de todos eles. Um currículo ou uma página web que
  apenas contém as informações necessárias, mas carece de organização visual,
  torna-se difícil de ler e pouco profissional. A aplicação conjunta de
  proximidade, alinhamento, repetição e contraste transforma um amontoado de
  dados em uma interface funcional e atraente. Observe como os princípios
  trabalham em conjunto em um projeto bem estruturado:
</p>

<ul>
  <li>
    <strong>Proximidade e Alinhamento:</strong> Agrupam informações relacionadas
    (como categorias de cursos ou blocos de experiência profissional) e as conectam
    por meio de eixos invisíveis, criando uma estrutura lógica e organizada.
  </li>
  <li>
    <strong>Repetição:</strong> Mantém a consistência visual através do uso padronizado
    de fontes, cores e pesos (como o uso constante de negrito para títulos), permitindo
    que o usuário identifique padrões rapidamente.
  </li>
  <li>
    <strong>Contraste:</strong> Destaca o que é prioritário, utilizando cores de
    fundo (como blocos azuis em fundos claros) ou variações tipográficas para separar
    diferentes seções e atrair o olhar para pontos-chave.
  </li>
</ul>

<p>
  Um exemplo prático é o portal de uma instituição de ensino: as modalidades de
  cursos são agrupadas (<strong>proximidade</strong>), distribuídas no topo da
  página (<strong>alinhamento</strong>), utilizam o mesmo estilo de fonte (<strong
    >repetição</strong
  >) e se destacam do restante do conteúdo por cores vibrantes (<strong
    >contraste</strong
  >). Essa harmonia visual é o que torna a navegação intuitiva para o usuário.
</p>
