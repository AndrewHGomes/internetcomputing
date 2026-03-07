<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Conceitos Fundamentais e Navegabilidade</h2>

<Audios modulo="M6" aulas={["13", "14", "15", "16"]} />

<p>
  A comunicação humana é complexa e baseada em representações simbólicas. Quando
  lemos uma palavra, criamos imagens mentais distintas baseadas em nossas
  vivências. No Web Design, o desafio é transpor essa subjetividade para um
  produto digital, criando um projeto visual que expresse conceitos de forma
  clara para um público diverso, permitindo que o usuário navegue e resolva
  problemas de forma autônoma.
</p>

<p>
  A <strong>Navegabilidade</strong> refere-se à fluidez com que se circula por um
  site e à facilidade com que as informações são localizadas. Ela deve ser intuitiva,
  tratando o ambiente digital como uma arquitetura física (semelhante a um shopping),
  onde fluxos e pontos de entrada devem ser planejados para facilitar o consumo e
  a localização de itens.
</p>

<h4>Benefícios da Boa Navegabilidade</h4>

<ul>
  <li>
    <strong>Experiência do Usuário:</strong> Torna a interação intuitiva, aumentando
    a satisfação e a retenção do visitante.
  </li>
  <li>
    <strong>Taxas de Conversão:</strong> Facilita o alcance de objetivos (como finalizar
    uma compra), impactando diretamente na geração de receita.
  </li>
  <li>
    <strong>SEO (Otimização para Buscadores):</strong> Melhora o ranqueamento em
    motores de busca, pois ajuda os rastreadores a entenderem a hierarquia e relevância
    do conteúdo.
  </li>
</ul>

<h4>Elementos Principais da Navegabilidade</h4>

<p>
  A organização da informação deve permitir que o usuário saiba sempre onde
  está, de onde veio e para onde pode ir. Os três pilares fundamentais são:
</p>

<ol>
  <li>
    <strong>Menus de Navegação:</strong> São os principais agrupadores de acesso
    ao conteúdo. Dividem-se em três tipos principais:
    <ul>
      <li>
        <strong>Horizontal:</strong> Comum no topo (cabeçalho), ideal para categorias
        principais em sites de página única ou blogs.
      </li>
      <li>
        <strong>Vertical:</strong> Localizado nas laterais, permite acomodar um volume
        maior de itens e subcategorias devido à rolagem da página.
      </li>
      <li>
        <strong>Hambúrguer:</strong> Ícone de três barras que expande o conteúdo;
        essencial para dispositivos móveis para economizar espaço, mas deve ser usado
        com cautela em desktops.
      </li>
    </ul>
  </li>
  <li>
    <strong>Mapa do Site (Sitemap):</strong> É a representação esquemática da estrutura
    do site. Serve tanto como guia para o usuário (geralmente no rodapé) quanto como
    ferramenta de planejamento para o designer organizar a hierarquia lógica das
    páginas.
  </li>
  <li>
    <strong>Consistência Visual:</strong> Envolve a manutenção de padrões de layout,
    cores, tipografia e posicionamento de elementos. A repetição desses padrões gera
    familiaridade, facilitando o reconhecimento da interface e a localização do usuário
    dentro do sistema.
  </li>
</ol>

<h3>Usabilidade</h3>

<p>
  Enquanto a navegabilidade foca no ato de circular, a <strong
    >usabilidade</strong
  > foca na eficácia com que o usuário alcança seus objetivos. Um site com boa usabilidade
  é aquele que cumpre as expectativas do visitante de forma eficiente, agradável
  e resolutiva, evitando que ele abandone a página por dificuldades técnicas ou funcionais.
</p>

<h4>Princípios Fundamentais</h4>

<ul>
  <li>
    <strong>Conhecimento do Público-alvo:</strong> Entender o nível de alfabetização
    digital e as necessidades dos usuários para ajustar o didatismo da interface.
  </li>
  <li>
    <strong>Navegação Intuitiva:</strong> Uso de menus claros e hierarquias bem definidas
    para facilitar a localização de informações.
  </li>
  <li>
    <strong>Acessibilidade:</strong> Inclusão de recursos para pessoas com necessidades
    especiais, como fontes legíveis, alto contraste e suporte a leitores de tela.
  </li>
  <li>
    <strong>Eficiência e Memorabilidade:</strong> O site deve permitir que as tarefas
    sejam feitas rapidamente (poucos cliques) e ser fácil de lembrar, facilitando
    o retorno do usuário.
  </li>
</ul>

<h4>Etapas de Implementação</h4>

<p>
  A aplicação da usabilidade no layout segue um processo estruturado em seis
  passos:
</p>

<ol>
  <li>
    <strong>Pesquisa de Usuários:</strong> Levantamento de requisitos e comportamentos
    do público-alvo.
  </li>
  <li>
    <strong>Prototipagem (Wireframe):</strong> Criação da estrutura visual básica
    e esquemática do site.
  </li>
  <li>
    <strong>Desenvolvimento de Conteúdo:</strong> Organização lógica de informações
    relevantes para sustentar a estrutura.
  </li>
  <li>
    <strong>Teste de Uso:</strong> Avaliação com usuários reais para identificar
    falhas e medir o grau de satisfação.
  </li>
  <li>
    <strong>Ajustes:</strong> Refinamento do projeto com base nos dados coletados
    nos testes.
  </li>
  <li>
    <strong>Monitoramento:</strong> Acompanhamento contínuo do site em uso real para
    melhorias futuras.
  </li>
</ol>

<h4>Diferença Prática: Navegabilidade vs. Usabilidade</h4>

<ul>
  <li>
    <strong>Navegabilidade:</strong> São as "galerias largas" de um shopping que
    permitem andar livremente.
  </li>
  <li>
    <strong>Usabilidade:</strong> É a "praça de alimentação" agrupada que permite
    ao usuário faminto encontrar rapidamente a solução para sua necessidade específica.
  </li>
</ul>

<h3>UX Design (User Experience Design)</h3>

<p>
  O <strong>UX Design</strong> é um campo multidisciplinar focado em criar experiências
  positivas e significativas na interação entre o usuário e produtos digitais. Ele
  integra navegabilidade e usabilidade, mas vai além, buscando evitar frustrações
  e promover satisfação tanto em tarefas funcionais (pagar uma conta) quanto emocionais
  (navegar em redes sociais).
</p>

<h4>Os Três Níveis do Design Emocional (Don Norman)</h4>

<p>
  A experiência do usuário é processada em diferentes profundidades psíquicas:
</p>

<ul>
  <li>
    <strong>Nível Visceral:</strong> Refere-se às reações instintivas e imediatas.
    É o impacto estético e sensorial inicial (o "primeiro olhar") que causa uma impressão
    instantânea.
  </li>
  <li>
    <strong>Nível Comportamental:</strong> Foca na experiência prática e no prazer
    de usar o produto. A satisfação surge quando o usuário consegue realizar suas
    tarefas com eficiência e sem erros.
  </li>
  <li>
    <strong>Nível Reflexivo:</strong> É o nível mais profundo, ligado ao significado,
    memórias e identidade. Relaciona-se ao valor que o usuário atribui ao produto
    e ao sentimento de conexão ou pertencimento.
  </li>
</ul>

<h4>Estratégia e Escopo no UX</h4>

<p>
  Para aplicar o UX Design de forma eficaz, o planejamento deve considerar três
  pilares estratégicos:
</p>

<ul>
  <li>
    <strong>Finalidade e Objetivos:</strong> O foco deve ser sempre a jornada do
    usuário. Em um e-commerce, por exemplo, o objetivo do UX não é apenas vender,
    mas garantir que o processo de compra seja o mais fácil e rápido possível.
  </li>
  <li>
    <strong>Funcionalidades (Escopo):</strong> Definição clara do que o site deve
    oferecer para atender às necessidades levantadas.
  </li>
  <li>
    <strong>Personas:</strong> Criação de perfis fictícios que representam os diferentes
    tipos de usuários do público-alvo. Elas servem para guiar as decisões de design,
    permitindo antecipar comportamentos e necessidades reais durante a navegação.
  </li>
</ul>

<p>
  O UX Design busca, em última análise, não apenas atender às expectativas do
  usuário, mas superá-las para gerar fidelização, mesmo considerando que fatores
  externos (como o estado emocional do visitante) influenciam a experiência.
</p>

<h3>Introdução às Redes de Computadores</h3>

<p>
  Uma rede de computadores é um conjunto de dispositivos interconectados
  (computadores, impressoras, roteadores) que trocam informações e compartilham
  recursos. Essa estrutura é a base da sociedade da informação, permitindo desde
  o acesso a um site até a conexão com máquinas de alta performance (<strong
    >mainframes</strong
  >).
</p>

<h4>Classificação por Extensão Geográfica</h4>

<p>As redes são classificadas principalmente pelo seu tamanho e alcance:</p>

<ul>
  <li>
    <strong>PAN (Personal Area Network):</strong> Rede pessoal para conectar dispositivos
    de um único usuário, como smartphones e laptops.
  </li>
  <li>
    <strong>LAN (Local Area Network):</strong> Rede local restrita a espaços pequenos,
    como residências, escritórios ou edifícios. É usada para compartilhar dados e
    periféricos.
  </li>
  <li>
    <strong>MAN (Metropolitan Area Network):</strong> Rede metropolitana que conecta
    áreas maiores, como campus universitários ou cidades, interligando várias LANs.
  </li>
  <li>
    <strong>WAN (Wide Area Network):</strong> Rede de longa distância que abrange
    cidades, países ou continentes.
  </li>
</ul>

<h4>Funcionamento e Componentes</h4>

<p>
  A comunicação em rede ocorre através da transmissão de <strong
    >pacotes de dados</strong
  >. Quando uma solicitação é feita, a informação é fragmentada em pacotes,
  transmitida e depois reagrupada no destino. Para que isso ocorra, são
  necessários:
</p>

<ul>
  <li>
    <strong>Dispositivos:</strong> Computadores, servidores e periféricos que compõem
    os pontos da rede.
  </li>
  <li>
    <strong>Equipamentos de Interconexão:</strong> Roteadores e switches, que direcionam
    o tráfego de dados para o destino correto.
  </li>
  <li>
    <strong>Meios de Transmissão:</strong> Caminhos físicos ou sem fio, como cabos,
    conectores e tecnologia Wi-Fi.
  </li>
  <li>
    <strong>Protocolos de Comunicação:</strong> Conjunto de regras e normas que validam
    e permitem que os dispositivos "falem a mesma língua" e troquem informações com
    segurança.
  </li>
</ul>

<h3>Arquitetura Cliente-Servidor e Protocolo HTTP</h3>

<p>
  A web opera majoritariamente no modelo de <strong
    >arquitetura Cliente-Servidor</strong
  >, uma estrutura centralizada onde o sistema é dividido em duas partes
  distintas que trocam funções entre si para entregar o conteúdo ao usuário.
</p>

<h4>O Funcionamento da Arquitetura</h4>

<ul>
  <li>
    <strong>Cliente:</strong> É o ponto de acesso (geralmente o navegador) que faz
    solicitações e processa as respostas recebidas para exibição ao usuário.
  </li>
  <li>
    <strong>Servidor:</strong> É a máquina de alta performance que armazena os conteúdos
    e bases de dados. Ele recebe as solicitações, processa-as e envia os dados de
    volta.
  </li>
  <li>
    <strong>Distribuição:</strong> Embora possam coexistir na mesma máquina, cliente
    e servidor geralmente estão em computadores distintos, permitindo a distribuição
    de carga de trabalho e o compartilhamento de recursos de um servidor com múltiplos
    clientes.
  </li>
</ul>

<h4>O Processo de Acesso a um Site</h4>

<p>Ao clicar em um link, ocorre uma cadeia de eventos técnica:</p>

<ol>
  <li>
    <strong>URL e DNS:</strong> O navegador identifica o endereço (URL) e
    consulta o <strong>DNS</strong> (Sistema de Nomes de Domínio) para converter
    o nome do site no endereço IP real do servidor.
  </li>
  <li>
    <strong>Conexão:</strong> O navegador estabelece conexão com o servidor através
    desse IP.
  </li>
  <li>
    <strong>Resposta do Servidor:</strong> O servidor localiza os arquivos solicitados
    em seu disco e os envia ao cliente.
  </li>
  <li>
    <strong>Exibição:</strong> O navegador recebe os dados, encerra a conexão e renderiza
    a página para o usuário.
  </li>
</ol>

<h4>Protocolo HTTP e Seus Métodos</h4>

<p>
  O <strong>HTTP (Hypertext Transfer Protocol)</strong> é o conjunto de regras
  que organiza essa troca de informações. Cada interação é composta por uma
  <strong>requisição</strong>
  (cliente) e uma <strong>resposta</strong> (servidor). As principais operações são
  realizadas através de métodos:
</p>

<ul>
  <li>
    <strong>GET:</strong> Solicita e recupera dados (ex: carregar os textos e imagens
    de uma página).
  </li>
  <li>
    <strong>POST:</strong> Envia dados para criar ou ajustar recursos no servidor
    (ex: preencher um formulário).
  </li>
  <li>
    <strong>PUT:</strong> Atualiza um recurso já existente, enviando apenas as modificações
    necessárias.
  </li>
  <li>
    <strong>DELETE:</strong> Solicita a remoção de um recurso específico do servidor.
  </li>
</ul>

<h3>Conclusão: Navegabilidade e Usabilidade</h3>

<p>
  A eficiência de um site depende da harmonia entre como o usuário circula (<strong
    >navegabilidade</strong
  >) e como ele realiza suas tarefas (<strong>usabilidade</strong>). Ambos são
  pilares para a satisfação do visitante e para o sucesso comercial (conversão)
  de um projeto digital.
</p>

<ul>
  <li>
    <strong>Navegabilidade (Onde estou?):</strong> Foca na facilidade de acesso à
    informação. O objetivo é a circulação intuitiva, idealmente permitindo encontrar
    o que se busca em até três cliques. Utiliza ferramentas como menus, sitemaps
    e padrões visuais constantes para guiar o usuário.
  </li>
  <li>
    <strong>Usabilidade (Como resolvo meu problema?):</strong> Foca na eficácia e
    acessibilidade. É a garantia de que o usuário conseguirá atingir seu objetivo
    de forma rápida e sem barreiras, independentemente de suas limitações ou do dispositivo
    utilizado.
  </li>
</ul>
