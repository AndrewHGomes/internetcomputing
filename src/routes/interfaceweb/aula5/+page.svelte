<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Interface e Experiência do Usuário (UX)</h2>

<Audios modulo="M4" aulas={["17", "18", "19", "20"]} />

<p>
  A criação de uma interface web vai além da estética; trata-se da <strong>
    complexa interação entre o ser humano e o que é exibido na tela
  </strong>. O objetivo central é desenvolver um ambiente onde o usuário se
  sinta confortável e consiga
  <strong>utilizar o sistema de forma eficiente</strong>. Projetar uma interface
  funcional exige desvendar os segredos por trás da experiência do usuário,
  garantindo que o diálogo entre a lógica da máquina e a compreensão humana seja
  fluido.
</p>

<h3>A Evolução Histórica da UX</h3>

<p>
  O conceito de UX (User eXperience) passou por diversas nomenclaturas e
  transformações tecnológicas ao longo das décadas para se tornar o que é hoje:
</p>

<ul>
  <li>
    <strong>Início (Eniac e Memex):</strong> Computadores eram puramente lógicos
    e mecânicos. Diferente de um motor físico, a lógica da máquina exigia uma "ponte"
    para ser compreendida. As primeiras interfaces eram físicas, baseadas em trocas
    de cabos e chaves (switches).
  </li>
  <li>
    <strong>Cartões Perfurados e Terminais:</strong> A IBM introduziu cartões perfurados
    para programação, um método complexo que foi substituído pelos primeiros monitores,
    onde já era possível digitar comandos. No entanto, o uso ainda era restrito a
    especialistas e engenheiros.
  </li>
  <li>
    <strong>Década de 1970 (O Microcomputador):</strong> Com a chegada dos computadores
    às pessoas comuns, surgiu a necessidade de instruções menos complexas. O laboratório
    Xerox PARC foi pioneiro na criação das interfaces gráficas para tornar a tecnologia
    acessível a leigos.
  </li>
  <li>
    <strong>Década de 1980 (Interação Homem-Computador):</strong> Cientistas de diversas
    áreas consolidaram o termo Interação Homem-Computador (IHC) para estudar como
    as pessoas lidavam com as máquinas.
  </li>
  <li>
    <strong>Década de 1990 (Design de Interação):</strong> O foco mudou para a "inter-ação"
    propriamente dita, priorizando o design do diálogo entre usuário e sistema.
  </li>
  <li>
    <strong>Século XXI (User eXperience):</strong> O termo UX consolidou-se como
    o padrão atual, abrangendo toda a experiência e percepção do usuário ao interagir
    com um produto ou serviço.
  </li>
</ul>

<h3>Conceito Fundamental do Design Centrado no Usuário</h3>

<p>
  Design, neste contexto, significa <strong>projeto</strong>. O objetivo é criar
  produtos compreensíveis e utilizáveis dentro dos limites tecnológicos. A
  premissa básica é que o usuário deve ser capaz de descobrir sozinho como
  operar o sistema, o que está acontecendo e quais ações tomar. Um bom design é
  aquele que exige o mínimo de instruções externas; quanto mais intuitivo,
  melhor.
</p>

<h4>Os Três Modelos Mentais</h4>

<p>
  Para que uma interface funcione, o designer deve equilibrar três visões
  diferentes:
</p>

<ul>
  <li>
    <strong>Modelo de Design:</strong> A ideia e os conceitos que o projetista tem
    em mente ao criar o sistema.
  </li>
  <li>
    <strong>Modelo do Usuário:</strong> A imagem mental que a pessoa comum forma
    ao interagir com o sistema.
  </li>
  <li>
    <strong>Imagem do Sistema:</strong> A parte visível e tátil (a interface). É
    através dela que o modelo do designer se comunica com o usuário. Se a imagem
    do sistema for falha, o usuário não entenderá a intenção do designer.
  </li>
</ul>

<h4>As 7 Regras de Norman para um Bom Design</h4>

<p>
  Baseado nos estudos de Donald Norman, existem diretrizes essenciais para
  garantir a usabilidade:
</p>

<ol>
  <li>
    <strong>Usar conhecimento de mundo:</strong> Aproveitar padrões que as pessoas
    já conhecem (ex: vermelho para "parar", verde para "seguir"). Quando a interface
    usa conceitos familiares, o aprendizado é simplificado.
  </li>
  <li>
    <strong>Simplificar a estrutura das tarefas:</strong> Minimizar o esforço do
    usuário. Isso pode ser feito através de mnemônicos (ajudas de memória), indicadores
    visuais de estado (como o painel de um carro), automação de rotinas ou simplificação
    da natureza da tarefa (ex: ouvir música via streaming vs. vinil).
  </li>
  <li>
    <strong>Tornar as coisas visíveis:</strong> Garantir que links, botões e funções
    importantes estejam destacados e fáceis de encontrar.
  </li>
  <li>
    <strong>Mapeamento:</strong> Criar uma relação clara entre a intenção do usuário,
    a ação realizada e o efeito no sistema. O feedback é crucial aqui: o sistema
    deve sempre reagir e informar que uma ação foi processada.
  </li>
  <li>
    <strong>Explorar coerções (restrições):</strong> Limitar as opções do usuário
    de forma que ele seja naturalmente guiado para a ação correta, reduzindo as chances
    de erro.
  </li>
  <li>
    <strong>Projetar para o erro:</strong> Partir do princípio que o usuário vai
    errar. O sistema deve permitir que o erro seja reconhecido e que o usuário consiga
    recuperar o estado anterior sem danos maiores.
  </li>
  <li>
    <strong>Padronização:</strong> Quando uma solução intuitiva não for possível,
    deve-se criar um padrão. Uma vez que o usuário aprende a regra do padrão, ele
    consegue replicar o conhecimento em todo o sistema.
  </li>
</ol>

<h3>Metas da Interface e da UX</h3>

<p>
  As metas de uma interface moderna vão além do funcional; elas buscam <strong>
    gerar uma conexão emocional e psicológica
  </strong> com o utilizador. Quanto mais dessas características um sistema reunir,
  maior será sua aceitação no mercado.
</p>

<ul>
  <li>
    <strong>Atributos de Experiência:</strong> Os sistemas devem ser projetados para
    serem satisfatórios, agradáveis, divertidos, interessantes e motivadores.
  </li>
  <li>
    <strong>Qualidade Visual e Criativa:</strong> A interface precisa ser agradável
    ao olhar, incentivando a criatividade e sendo emocionalmente adequada ao contexto
    de uso.
  </li>
  <li>
    <strong>Valor Percebido:</strong> O sistema deve ser útil e compensador, fazendo
    com que o usuário sinta que o tempo investido na interação valeu a pena.
  </li>
</ul>

<h4>Interdependência das Metas</h4>

<p>
  As metas de UX não funcionam de forma isolada, mas sim de maneira integrada e
  dependente:
</p>

<ul>
  <li>
    <strong>Eficiência e Emoção:</strong> Para que um sistema seja considerado emocionalmente
    adequado e compensador, ele precisa ser eficiente no uso.
  </li>
  <li>
    <strong>Motivação e Utilidade:</strong> Um usuário só se sente motivado a utilizar
    uma ferramenta se ela possuir uma utilidade clara.
  </li>
  <li>
    <strong>Interesse e Compreensão:</strong> Para que algo seja percebido como interessante,
    deve ser, antes de tudo, fácil de entender e navegar.
  </li>
</ul>

<p>
  O exemplo clássico dessa integração é o <strong>Instagram</strong>, que
  combina apelo visual, facilidade de uso e recompensas emocionais para manter o
  engajamento do usuário.
</p>

<h3>A Lei de Krug: "Não me faça pensar"</h3>

<p>
  A premissa central é que a interface deve ser <strong>autoexplicativa</strong
  >. Quando um usuário acessa um site ou aplicativo, ele não deseja gastar
  energia mental tentando entender como a ferramenta funciona; ele quer apenas
  consumir o conteúdo ou realizar uma tarefa.
</p>

<ul>
  <li>
    <strong>A Interface "Invisível":</strong> A interface deve desaparecer para o
    usuário. Em redes sociais como Instagram ou TikTok, o foco é o conteúdo (fotos/vídeos),
    e não os botões ou a navegação.
  </li>
  <li>
    <strong>Evidência e Simplicidade:</strong> Tudo deve ser óbvio, simples e direto.
    Se o usuário precisa parar para pensar em qual botão clicar, o design falhou.
  </li>
  <li>
    <strong>Acessibilidade Universal:</strong> O projeto deve ser tão claro que até
    pessoas sem experiência tecnológica consiga utilizá-lo sem dificuldades ou traumas.
  </li>
</ul>

<h4>Impacto Comercial e Confiança</h4>

<p>
  A complexidade de uma interface tem consequências diretas no sucesso de um
  produto digital:
</p>

<ul>
  <li>
    <strong>Taxa de Conversão:</strong> Existe uma relação comercial direta entre
    simplicidade e consumo. Se um site exige muitos cliques para chegar a um produto,
    o usuário desiste da compra.
  </li>
  <li>
    <strong>Acúmulo de Distrações:</strong> Cada pequena dúvida gera trabalho mental.
    O somatório dessas distrações leva ao abandono do site ou à desinstalação do
    aplicativo em favor de uma alternativa mais simples.
  </li>
  <li>
    <strong>Credibilidade:</strong> Interfaces confusas transmitem uma imagem de
    desleixo. Quando o desenvolvedor não torna a navegação óbvia, o usuário perde
    a confiança na marca ou no sistema.
  </li>
</ul>

<h4>O Papel do Projetista</h4>

<p>
  Como projetista de interface, sua meta é priorizar a finalidade do site acima
  da própria estrutura visual:
</p>

<ul>
  <li>
    <strong>Site de Vendas:</strong> O destaque deve ser total para os produtos.
  </li>
  <li>
    <strong>Site de Jogos:</strong> A prioridade é a diversão e a facilidade de iniciar
    a partida.
  </li>
  <li>
    <strong>Site de Informação:</strong> A notícia ou o dado deve estar sempre em
    primeiro plano.
  </li>
</ul>

<p>
  O sucesso do design é medido pela rapidez com que o usuário atinge seu
  objetivo sem precisar "decifrar" a tela.
</p>

<h3>O Conceito de "Satisfazimento" (Satisficing)</h3>

<p>
  O termo, uma junção de "satisfazer" com "otimizar", indica que os usuários não
  buscam a <strong>melhor</strong> opção disponível em uma interface, mas sim a
  <strong> primeira opção razoável </strong> que encontram. Em vez de lerem a página
  inteira para tomar uma decisão perfeita, eles clicam no que parece ser "bom o suficiente"
  para resolver seu problema imediato.
</p>

<h4>Por que os usuários não escolhem a melhor opção?</h4>

<p>
  Steve Krug aponta quatro motivos principais para esse comportamento impulsivo
  e prático:
</p>

<ul>
  <li>
    <strong>Pressa constante:</strong> Vivemos em uma era de aceleração do tempo.
    O usuário quer resolver sua tarefa o mais rápido possível e não tem paciência
    para análises profundas.
  </li>
  <li>
    <strong>Baixo custo do erro:</strong> Na internet, errar raramente traz consequências
    graves. Se o usuário clicar no botão errado, basta clicar em "voltar" e tentar
    novamente. Não há punição real.
  </li>
  <li>
    <strong>Dificuldade de avaliação:</strong> Em sistemas mal projetados, analisar
    todas as opções não garante uma escolha melhor. O esforço mental para entender
    uma interface confusa muitas vezes não vale a pena.
  </li>
  <li>
    <strong>Adivinhar é mais fácil:</strong> Para a maioria das pessoas, "chutar"
    e ver o que acontece é mais divertido e exige menos trabalho do que ler manuais
    ou instruções detalhadas.
  </li>
</ul>

<h4>Implicações para o Design</h4>

<p>
  Entender o "satisfazimento" reforça que o projetista deve criar interfaces
  onde a "primeira opção razoável" seja, de preferência, a ação correta. Se o
  usuário vai apenas "bater o olho" e clicar, os elementos mais importantes
  devem ter o maior peso visual e clareza imediata.
</p>

<h3>Conclusão</h3>

<p>
  Terminamos esta etapa, em que tratamos um pouco da história da UX, desde a
  interação homem-computador até hoje. Depois, vimos um pouco do design centrado
  no usuário e a necessidade de deixar visíveis comandos e possibilidades, entre
  outras tantas coisas que foram ali discutidas. Para deixar tudo bem simples,
  apresentamos todas as regras do Donald Norman, que funcionam para UX de
  qualquer produto ou serviço.
</p>

<p>
  Adiante, vimos as metas da UX e das interfaces, para deixar o sistema ou o
  site melhores e mais atrativos para nossos usuários. Discutimos também a regra
  de não pensar, que nossos usuários utilizam o tempo todo, e logo em seguida,
  vimos a regra do satisfazimento.
</p>
