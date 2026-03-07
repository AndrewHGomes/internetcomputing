<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Introdução à Animação e Modelagem 3D</h2>

<Audios modulo="M7" aulas={["17", "18", "19", "20"]} />

<p>
  A compreensão da animação 3D exige o domínio de conceitos que vão desde os
  princípios da animação tradicional até as habilidades técnicas de modelagem
  digital. O processo envolve a criação de objetos no espaço, a estruturação de
  personagens, a definição de cenários e a aplicação de texturas e materiais
  para compor o ambiente visual.
</p>

<h3>Os 12 Princípios da Animação</h3>

<p>
  Originalmente descritos por animadores da Disney, estes princípios fundamentam
  tanto a animação 2D quanto a 3D, garantindo realismo e expressividade aos
  movimentos:
</p>

<ul>
  <li>
    <strong>Esticar e comprimir (Squash and Stretch):</strong> Dá a sensação de peso
    e flexibilidade aos objetos.
  </li>
  <li>
    <strong>Antecipação:</strong> Prepara a audiência para uma ação que está prestes
    a ocorrer.
  </li>
  <li>
    <strong>Encenação (Staging):</strong> Direciona a atenção do espectador para
    o que é importante na cena.
  </li>
  <li>
    <strong>Siga direto e pose a pose:</strong> Define se a animação é feita quadro
    a quadro ou por poses principais.
  </li>
  <li>
    <strong>Prosseguimento e ação de sobreposição:</strong> Mostra como partes do
    corpo continuam se movendo após o fim de uma ação.
  </li>
  <li>
    <strong>Começar e terminar devagar (Slow in and slow out):</strong> Reflete a
    aceleração e desaceleração natural dos movimentos físicos.
  </li>
  <li>
    <strong>Arcos:</strong> Segue a trajetória curva natural da maioria dos movimentos
    orgânicos.
  </li>
  <li>
    <strong>Ação secundária:</strong> Adiciona movimentos menores que apoiam e enriquecem
    a ação principal.
  </li>
  <li>
    <strong>Cronometragem (Timing):</strong> Ajusta a velocidade do movimento para
    definir peso, personalidade e humor.
  </li>
  <li>
    <strong>Exagero:</strong> Intensifica as características e ações para tornar
    a animação mais atraente.
  </li>
  <li>
    <strong>Desenhar sólidos:</strong> Garante que os objetos pareçam ter volume,
    peso e profundidade no espaço 3D.
  </li>
  <li>
    <strong>Apelo (Appeal):</strong> Cria personagens e poses que sejam visualmente
    interessantes e cativantes.
  </li>
</ul>

<h4>O Papel do Modelador Digital</h4>

<p>
  A modelagem digital 3D consiste em criar representações matemáticas que
  simulam o formato de objetos tridimensionais. Embora utilize softwares
  complexos, a base do trabalho é artística, frequentemente partindo de esboços
  em papel, referências do mundo real ou esculturas físicas em argila. Para
  atuar na área, o modelador deve desenvolver competências fundamentais que vão
  além do domínio técnico:
</p>

<ul>
  <li>
    <strong>Bagagem de Referências:</strong> Capacidade de mesclar elementos do mundo
    real para criar personagens e objetos fictícios de forma convincente.
  </li>
  <li>
    <strong>Observação Aguçada:</strong> Habilidade para identificar detalhes como
    texturas, simetria, separação de peças e comportamentos físicos dos materiais.
  </li>
  <li>
    <strong>Resolução de Problemas:</strong> Competência para encontrar soluções
    visuais e técnicas durante a construção das formas e estruturas dos modelos.
  </li>
</ul>

<h3>Transformações Espaciais</h3>

<p>
  As transformações controlam como os elementos de uma malha poligonal se
  relacionam no espaço 3D, operando através de matrizes de transformação
  aplicadas a vetores de posição. Qualquer software de modelagem oferece três
  operações fundamentais:
</p>

<ul>
  <li>
    <strong>Mover:</strong> Reposicionamento do objeto para um local específico nos
    eixos tridimensionais.
  </li>
  <li>
    <strong>Rotacionar:</strong> Giro do objeto em torno de um eixo central, definido
    por ângulos.
  </li>
  <li>
    <strong>Escalar:</strong> Alteração do tamanho do objeto, aumentando ou diminuindo
    suas proporções.
  </li>
</ul>

<h4>Estrutura e Mapas de Vértices</h4>

<p>
  A modelagem básica organiza-se a partir de pontos (vértices) conectados por
  arestas (edges) para formar polígonos. O "peso da aresta" determina se os
  cantos serão nítidos ou suaves, enquanto os splines garantem construções e
  movimentos mais orgânicos. Para organizar as informações do modelo,
  utilizam-se os <strong>Mapas de Vértices (vortex maps)</strong>:
</p>

<ul>
  <li>
    <strong>Mapa de Textura (UV):</strong> Planifica a superfície para a aplicação
    de imagens.
  </li>
  <li>
    <strong>Mapa de Peso (Weight):</strong> Define a influência de estruturas internas
    (ossos) sobre a malha.
  </li>
  <li>
    <strong>Mapa de Transformação (Morph):</strong> Armazena dados de deslocamento
    para deformações.
  </li>
  <li>
    <strong>Mapa de Seleção:</strong> Agrupa informações sobre pontos específicos.
  </li>
  <li>
    <strong>Mapa de Cor:</strong> Guarda valores de variação cromática no objeto.
  </li>
</ul>

<h4>Técnicas de Modelagem Realística</h4>

<p>
  A evolução dos softwares consolidou diferentes métodos para a criação de
  superfícies digitais, variando conforme a necessidade de suavidade ou
  detalhamento:
</p>

<ul>
  <li>
    <strong>NURBS:</strong> Utiliza curvas matemáticas suaves (B-Splines). Foi muito
    usada nos anos 90, mas perdeu espaço por ser complexa para modelagem orgânica.
  </li>
  <li>
    <strong>Modelagem Poligonal:</strong> É a técnica mais comum atualmente. Trabalha
    com subdivisões que definem o nível de detalhamento, classificados como High
    Poly (alto detalhe) ou Low Poly (baixo detalhe).
  </li>
  <li>
    <strong>Subdivisão de Superfície (Subdivision Surface):</strong> Um refinamento
    da modelagem poligonal que gera superfícies perfeitamente lisas a partir de uma
    malha de polígonos.
  </li>
</ul>

<h3>Técnicas de Movimentação e Estrutura 3D</h3>

<p>
  O processo de preparação de um modelo para animação ocorre logo após a
  finalização da malha poligonal. O modelador entrega a estrutura geométrica,
  que então recebe referências visuais e sistemas de articulação para permitir o
  movimento.
</p>

<h4>Blueprints</h4>

<p>
  Os blueprints são guias visuais que auxiliam o animador a manter a
  consistência do modelo durante a criação. Eles funcionam como um mapa de
  referência técnica, geralmente apresentando o personagem em múltiplas vistas
  (frente, costas e laterais).
</p>

<ul>
  <li>
    <strong>Função:</strong> Ajudam a definir proporções e posições de movimento
    (corrida, salto, caminhada).
  </li>
  <li>
    <strong>Limitações:</strong> Auxiliam na definição de limites de velocidade,
    altura de saltos e expressões faciais.
  </li>
  <li>
    <strong>Praticidade:</strong> Podem ser importados diretamente para o software
    de modelagem, facilitando o desenvolvimento a partir de modelos já existentes.
  </li>
</ul>

<h4>Rigging e Estruturas Articuladas</h4>

<p>
  O <strong>Rigging</strong> é a criação de um sistema de articulações e
  músculos que permite a movimentação do modelo. Ele funciona através de uma
  hierarquia de parentesco (<strong>Parenting</strong>), onde o objeto "filho"
  pode se mover sozinho, mas segue obrigatoriamente todos os movimentos do
  objeto "pai" (ex: se o ombro move, a mão acompanha).
</p>

<ul>
  <li>
    <strong>Componentes da Estrutura:</strong>
    <ul>
      <li>
        <strong>Articulações (Joints):</strong> Pontos de conexão e dobra.
      </li>
      <li><strong>Ossos (Bones):</strong> Unem visualmente as articulações.</li>
      <li>
        <strong>Pivôs (Pivots):</strong> Marcadores que definem o ponto exato de
        rotação.
      </li>
      <li>
        <strong>Músculos (Muscles):</strong> Sistemas que simulam deformações reais
        na malha conforme os ossos se movem.
      </li>
    </ul>
  </li>
  <li>
    <strong>Sistemas de Movimentação:</strong>
    <ul>
      <li>
        <strong>Cinemática Direta (FK):</strong> O movimento segue a ordem natural
        da hierarquia (do pai para o filho).
      </li>
      <li>
        <strong>Cinemática Inversa (IK):</strong> Inverte a lógica, onde mover a
        extremidade (como a mão) faz com que todo o braço se ajuste automaticamente.
      </li>
      <li>
        <strong>Sonda e Deformadores:</strong> Funcionam como fios de marionete,
        conectando o sistema de controle à geometria do personagem para gerar efeitos
        como dobras de pele e tecidos.
      </li>
    </ul>
  </li>
</ul>

<h3>Movimentação de Personagens</h3>

<p>
  A animação de personagens exige um conhecimento básico de anatomia para
  garantir verossimilhança, mesmo em criaturas fictícias. O foco principal
  reside na compreensão das estruturas ósseas e musculares para replicar
  movimentos naturais.
</p>

<h4>Expressões Faciais</h4>

<p>
  A face humana possui 22 ossos, sendo que a maioria (exceto a mandíbula)
  permanece estática durante as expressões. O movimento facial é ditado
  principalmente pelos músculos; por isso, a malha poligonal deve seguir o fluxo
  da musculatura real.
</p>

<ul>
  <li>
    <strong>Manipulação:</strong> Embora seja possível mover vértices individualmente,
    os animadores utilizam o rigging facial para controlar grupos de vértices simultaneamente.
  </li>
  <li>
    <strong>Blendshapes:</strong> Técnica que permite criar cópias da cabeça em diferentes
    "poses-chave" (expressões prontas) para transitar entre elas de forma fluida.
  </li>
</ul>

<h4>Técnicas de Movimentação</h4>

<p>
  Para evitar a sensação de estranheza no público, a movimentação de pessoas e
  animais deve ser orgânica. As principais técnicas para alcançar esse resultado
  são:
</p>

<ul>
  <li>
    <strong>Quadro-chave (Keyframing):</strong> Define as posições iniciais, intermediárias
    e finais de uma ação. O software calcula a transição entre esses pontos, evitando
    a necessidade de desenhar manualmente cada um dos 24 a 30 quadros por segundo.
  </li>
  <li>
    <strong>Animação com Gráficos:</strong> Utiliza curvas de trajetória e gráficos
    de interpolação para ajustar a velocidade e a sutileza do movimento entre dois
    quadros-chave.
  </li>
  <li>
    <strong>Captura de Movimento (Motion Capture):</strong> Registra o movimento
    de um ator real através de sensores e marcadores estratégicos. Esses dados são
    transferidos para o modelo digital, garantindo um realismo de alto nível, comum
    em filmes e jogos modernos.
  </li>
</ul>

<h3>Cenários, Texturas e Materiais</h3>

<p>
  A criação de cenários 3D vai além da estética, cumprindo funções narrativas e
  técnicas como explicar relações espaciais, criar atmosferas emocionais,
  realçar o papel do personagem e controlar a composição visual e o impacto da
  cena.
</p>

<h4>Modelagem de Ambientes Urbanos</h4>

<p>
  Espaços urbanos exigem áreas extensas sem repetições excessivas. A simetria e
  padronização das cidades facilitam a criação de modelos-base. Para garantir
  qualidade, deve-se considerar:
</p>

<ul>
  <li>
    <strong>Perspectiva:</strong> Define o ponto de vista (primeira pessoa, terceira
    pessoa, isométrica ou top-down).
  </li>
  <li>
    <strong>Tema:</strong> Define a "personalidade" da cidade (suja, futurista, litorânea).
  </li>
  <li>
    <strong>Tamanho e Escala:</strong> Ajuste do mapa de texturas e proporção correta
    entre o mundo e o personagem.
  </li>
</ul>

<h4>Métodos de Construção:</h4>

<ol>
  <li>
    <strong>Modular:</strong> Construção sobre um grid (grade), onde quarteirões
    e prédios se encaixam como peças.
  </li>
  <li>
    <strong>Livre:</strong> Objetos distribuídos conforme a visão do espectador,
    sem seguir uma grade rígida.
  </li>
  <li>
    <strong>Híbrido:</strong> Combina os dois métodos, usando módulos para prédios
    e distribuição livre para detalhes.
  </li>
</ol>

<h4>Modelagem de Ambientes Naturais</h4>

<p>
  Diferente do urbano, o ambiente natural é rico em detalhes orgânicos e
  ecossistemas variados. Seus elementos principais incluem:
</p>

<ul>
  <li>
    <strong>Terreno:</strong> Criado com polígonos e pixels em softwares 3D ou editores
    de jogos.
  </li>
  <li>
    <strong>Água:</strong> Complexa de simular, pois exige cálculos de dinâmica de
    fluidos.
  </li>
  <li>
    <strong>Céu:</strong> Pode ser uma imagem simples, um
    <strong>Sky-dome</strong> (cúpula que envolve o mundo) ou um Sky-box (cubo mapeado).
  </li>
  <li>
    <strong>Iluminação (Sol):</strong> Tratado tecnicamente como uma
    <strong>luz direcional</strong>
    e não apenas como um objeto sólido.
  </li>
  <li>
    <strong>Vegetação:</strong> Uso de plantas e árvores para preencher o terreno
    e ditar o tom da cena (ex: árvores secas para apreensão).
  </li>
</ul>

<h4>Texturas e Materiais</h4>

<p>
  Após a modelagem e o rigging, o artista de texturas transforma as superfícies
  lisas em representações realistas ou conceituais.
</p>

<ul>
  <li>
    <strong>Mapa UV:</strong> Processo de "planificar" a superfície 3D para que uma
    imagem 2D (textura) possa ser aplicada com precisão sobre ela.
  </li>
  <li>
    <strong>Sombreadores (Shaders):</strong> Comandos que dizem ao software como
    calcular a luz. Eles definem cor, refletividade, transparência, refração e brilho.
  </li>
  <li>
    <strong>Simulação de Superfície:</strong> Desenvolvimento de padrões (fractais,
    gradientes, xadrez) para dar aos materiais propriedades visuais específicas antes
    da renderização final.
  </li>
</ul>

<h3>Conclusão: Fluxo de Produção</h3>

<p>
  O processo de criação em computação gráfica e animação segue uma ordem lógica
  de desenvolvimento:
</p>

<ul>
  <li>
    <strong>O Modelador e a Gênese do Objeto:</strong> O trabalho começa com o modelador,
    que transforma referências e conceitos artísticos em malhas poligonais através
    de transformações espaciais (mover, rotacionar, escalar).
  </li>
  <li>
    <strong>Estruturação e Movimento:</strong> Com o modelo pronto, aplicam-se técnicas
    de movimentação (rigging, quadros-chave e cinemática). Estas técnicas são fundamentais
    para dar vida e expressividade, permitindo que personagens (humanos ou animais)
    manifestem emoções através de expressões faciais e movimentos corporais verossímeis.
  </li>
  <li>
    <strong>Ambientação e Contexto:</strong> O personagem é inserido em cenários
    (urbanos ou naturais), cada um com suas regras de construção (modular ou livre)
    e desafios técnicos específicos (como a simulação de água e vegetação).
  </li>
  <li>
    <strong>Finalização Visual:</strong> O realismo e a imersão são atingidos na
    etapa final, com a aplicação de texturas via mapas UV e a configuração de materiais
    através de shaders, que definem como a luz interage com as superfícies.
  </li>
</ul>
