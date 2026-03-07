<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Introdução ao Desenvolvimento Web</h2>

<Audios modulo="M6" aulas={["21", "22", "23", "24"]} />

<p>
  A interface gráfica de um site é a representação visual que permite a
  interação com o usuário. Sem ela, a navegação seria restrita à leitura de
  linhas de código. O desenvolvimento profissional de portais exige métodos
  eficientes para estruturar regras visuais amplas, evitando o trabalho manual
  exaustivo de codificar elemento por elemento. Os principais tópicos para o
  desenvolvimento e publicação de um site incluem:
</p>

<ul>
  <li>CSS (Estilização);</li>
  <li>Prototipagem e teste;</li>
  <li>Registro de domínio;</li>
  <li>Publicação e hospedagem;</li>
  <li>Protocolo FTP.</li>
</ul>

<h3>HTML: A Base da Estrutura</h3>

<p>
  Os navegadores funcionam como interpretadores que transformam códigos de
  marcação em interfaces visuais. O HTML (HyperText Markup Language) é a
  linguagem predominante, utilizada para definir a ordem, a hierarquia e a
  estrutura do conteúdo por meio de <strong>tags</strong> e
  <strong>atributos</strong>.
</p>

<p>
  Um exemplo prático é a criação de títulos. Para um título principal,
  utiliza-se a tag &lt;h1&gt;. Caso seja necessário aplicar estilos diretamente
  no HTML (estilo in-line), o código seria: &lt;h1 style="font-family: 'Times
  New Roman', serif; color: yellow;"&gt; Este é o título &lt;/h1&gt;.
</p>

<h3>CSS: Linguagem de Estilo</h3>

<p>
  O <strong>CSS (Cascading Style Sheets)</strong> é uma linguagem de estilo utilizada
  para definir como os elementos HTML devem ser exibidos em diferentes mídias. Sua
  principal vantagem é a economia de trabalho, permitindo que uma única regra altere
  centenas de páginas simultaneamente, estabelecendo uma hierarquia de "leis" que
  o navegador deve seguir. Existem três formas de aplicar o CSS:
</p>

<ul>
  <li><strong>In-line:</strong> dentro da tag HTML usando o atributo style;</li>
  <li>
    <strong>Interna:</strong> dentro da seção &lt;head&gt; da página, utilizando
    a tag &lt;style&gt;;
  </li>
  <li>
    <strong>Externa:</strong> através de um arquivo .css independente e vinculado
    ao documento.
  </li>
</ul>

<h4>Estrutura e Componentes do CSS</h4>

<p>
  Para padronizar elementos, como definir que todos os títulos &lt;h1&gt; sejam
  azuis e em fonte Arial, utiliza-se a sintaxe: h1 &lcub; font-family: Arial;
  color: blue; &rcub;. A estrutura do CSS é dividida em quatro componentes
  fundamentais:
</p>

<ul>
  <li>
    <strong>Seletor:</strong> indica qual elemento HTML será estilizado (ex: h1,
    p, body);
  </li>
  <li>
    <strong>Declaração:</strong> define as propriedades e valores que serão aplicados
    (ex: color: blue);
  </li>
  <li>
    <strong>Regras:</strong> o conjunto formado pelo seletor e suas declarações,
    sempre delimitados por chaves &lcub; &rcub;;
  </li>
  <li>
    <strong>Comentários:</strong> anotações que explicam a lógica do código, invisíveis
    ao usuário final. São escritos entre /* e */ (ex: /* Estilo dos títulos */).
  </li>
</ul>

<h3>Editores de Páginas e Ferramentas de Criação</h3>

<p>
  A criação de páginas web segue uma estrutura lógica universal: o navegador
  solicita dados ao DNS, que consulta o servidor, retornando as informações que
  o navegador interpreta e exibe. Embora seja tecnicamente possível criar um
  site inteiro usando apenas um <strong>bloco de notas</strong> (salvando o arquivo
  com a extensão .html), o mercado utiliza ferramentas avançadas para otimizar a
  produtividade e a complexidade dos projetos.
</p>

<h3>Desenvolvimento Profissional e Design</h3>

<p>
  O fluxo de trabalho profissional geralmente se divide entre a criação do <strong
  >
    plano visual
  </strong>
  (layout) e a <strong>codificação</strong> (HTML/CSS). Para o design, utilizam-se
  softwares que exportam layouts ou preparam os elementos gráficos:
</p>

<ul>
  <li>
    <strong>Softwares Pagos:</strong> Photoshop (imagens raster/layouts), Illustrator
    (vetores) e Corel Draw (vetores e logos).
  </li>
  <li>
    <strong>Softwares Livres (Gratuitos):</strong> Gimp (alternativa ao Photoshop)
    e Inkscape (alternativa ao Illustrator).
  </li>
</ul>

<h3>Editores de Código e IDEs</h3>

<p>
  Diferente dos softwares de design, os editores de páginas focam na organização
  do código e na interação dos elementos. Eles oferecem bibliotecas de códigos e
  recursos de <strong>autocompletar</strong>, que agilizam a escrita das
  linguagens.
</p>

<ul>
  <li>
    <strong>Adobe Dreamweaver:</strong> Permite o gerenciamento completo de projetos.
    Possui tanto um editor de código puro quanto uma interface "arrastar e soltar"
    para quem tem menos afinidade com a sintaxe.
  </li>
  <li>
    <strong>Visual Studio Code (VS Code):</strong> Atualmente é um dos editores mais
    utilizados por desenvolvedores no mundo, focado na escrita de código-fonte de
    alto desempenho.
  </li>
</ul>

<h3>Plataformas Online (Construtores de Sites)</h3>

<p>
  Para quem busca agilidade ou não possui conhecimentos técnicos em programação,
  existem plataformas baseadas em templates pré-diagramados. Elas automatizam a
  criação do código enquanto o usuário manipula o visual.
</p>

<ul>
  <li>
    <strong>Exemplos:</strong> Wix, Squarespace e WordPress (versão online).
  </li>
  <li>
    <strong>Vantagens:</strong> Facilidade de uso, interface visual intuitiva e pacotes
    integrados com hospedagem.
  </li>
  <li>
    <strong>Limitações:</strong> Menor flexibilidade para customizações profundas
    via código e dificuldades na integração com sistemas empresariais internos complexos.
  </li>
</ul>

<h3>Gerenciadores de Conteúdo (CMS)</h3>

<p>
  Após a criação e publicação de um site, a manutenção de conteúdos (como
  notícias ou blogs) precisa ser ágil e acessível. Antigamente, qualquer
  alteração exigia a edição manual do HTML e o envio via FTP. Para resolver
  isso, surgiram os <strong>CMS (Content Management Systems)</strong>,
  plataformas que permitem gerenciar e publicar conteúdo digital sem a
  necessidade de conhecimentos técnicos em programação.
</p>

<h4>Funcionalidade e Dinâmica de Trabalho</h4>

<p>
  O CMS atua como uma interface amigável que facilita a entrega de documentos
  complexos. No mercado profissional, o webdesigner geralmente utiliza um CMS
  como base estrutural para construir o site, entregando ao cliente final o
  acesso apenas à área administrativa para atualizações de rotina.
</p>

<ul>
  <li>
    <strong>Autonomia:</strong> Permite que funcionários de uma empresa atualizem
    dados sem contratar o designer para cada nova postagem.
  </li>
  <li>
    <strong>Segurança e Controle:</strong> O desenvolvedor pode criar níveis de acesso,
    limitando o cliente à edição de textos e imagens, impedindo alterações acidentais
    no layout ou no código-fonte.
  </li>
  <li>
    <strong>Eficiência:</strong> Elimina o fluxo manual de abrir editores de código
    e realizar transferências de arquivos para atualizações simples.
  </li>
</ul>

<h4>Principais Plataformas CMS</h4>

<p>
  Existem diversas opções de sistemas de código aberto (Open Source) que servem
  tanto para a criação quanto para a ancoragem de conteúdos:
</p>

<ul>
  <li>
    <strong>WordPress:</strong> O sistema mais tradicional e utilizado no mundo.
    É instalado no servidor e serve como base para portais robustos.
  </li>
  <li>
    <strong>Outras Opções:</strong> Joomla!, Ghost, Jekyll, Craft CMS e Serendipity.
  </li>
  <li>
    <strong>Modelos Integrados:</strong> Plataformas como Wix e Squarespace também
    atuam como CMS, mas unem a criação visual ao gerenciamento de conteúdo em um
    ambiente fechado.
  </li>
</ul>

<h3>Registro de Domínio e Hospedagem</h3>

<p>
  Um site só está efetivamente concluído quando está publicado e funcional. Para
  isso, são necessários dois pilares: o <strong>domínio</strong> (o endereço
  digital) e a
  <strong>hospedagem</strong> (o espaço físico no servidor).
</p>

<h4>Domínio: O Endereço Digital</h4>

<p>
  O domínio é a identidade do site na barra de endereços do navegador. Ele
  facilita o acesso ao converter endereços IP complexos em nomes memoráveis.
</p>

<ul>
  <li>
    <strong>Composição:</strong> É formado pelo <strong>nome</strong> (marca ou
    essência do projeto) e pela <strong>extensão</strong> (que indica o tipo de organização
    ou localização, como .adv.br para advogados ou .org para ONGs).
  </li>
  <li>
    <strong>Boas Práticas:</strong> Deve ser curto, fácil de digitar e evitar palavras
    complexas.
  </li>
  <li>
    <strong>Registro:</strong> No Brasil, o <strong>Registro.BR</strong> é o órgão
    principal para verificar disponibilidade. O registro tem prazo de validade e
    precisa de renovação periódica para não ser perdido.
  </li>
</ul>

<h4>Hospedagem: O Espaço de Armazenamento</h4>

<p>
  Se o domínio é o endereço, a hospedagem é o "terreno" onde os arquivos do site
  ficam guardados. É um serviço que mantém os dados em um servidor conectado à
  internet 24h por dia.
</p>

<h4>Tipos de Hospedagem</h4>

<ul>
  <li>
    <strong>Gratuita:</strong> Indicada apenas para testes; possui baixa segurança
    e recursos limitados.
  </li>
  <li>
    <strong>Compartilhada:</strong> Vários sites dividem o mesmo servidor. É econômica,
    mas o tráfego de um site pode afetar a velocidade dos outros. Ideal para pequenos
    sites e blogs.
  </li>
  <li>
    <strong>Servidor Virtual Privado (VPS):</strong> Uma máquina física é dividida
    em servidores virtuais independentes, oferecendo melhor performance que a compartilhada.
  </li>
  <li>
    <strong>Dedicada:</strong> Um servidor exclusivo para um único site. Oferece
    máxima segurança e desempenho, porém com custo elevado.
  </li>
  <li>
    <strong>Em Nuvem (Cloud):</strong> Utiliza vários servidores interconectados
    para equilibrar a carga. É altamente escalável e flexível para sites com grandes
    picos de acesso.
  </li>
</ul>

<h4>Critérios para Escolha</h4>

<p>
  Ao contratar um serviço de hospedagem (especialmente para sites fora de
  construtores como Wix), deve-se avaliar:
</p>

<ul>
  <li>
    <strong>Velocidade e Uptime:</strong> O tempo que o servidor permanece online
    e a rapidez na resposta.
  </li>
  <li>
    <strong>Recursos:</strong> Espaço em disco, limite de tráfego de dados e contas
    de e-mail inclusas.
  </li>
  <li>
    <strong>Suporte Técnico:</strong> Disponibilidade de atendimento para resolver
    falhas.
  </li>
  <li>
    <strong>Independência:</strong> Plataformas fechadas (Wix/Squarespace) não permitem
    migrar o site para outros servidores facilmente, o que pode ser uma desvantagem
    estratégica.
  </li>
</ul>

<h3>Protocolo FTP</h3>

<p>
  Para sites desenvolvidos localmente (em vez de plataformas online), é
  necessário enviar os arquivos do computador para o servidor de hospedagem. O
  método padrão para essa tarefa é o <strong
    >FTP (File Transfer Protocol)</strong
  >, um protocolo de rede que estabelece as regras para o acesso e a
  transferência de dados entre dispositivos conectados.
</p>

<h4>Origem e Segurança</h4>

<p>
  Criado na década de 1970 por Abhay Bhushan (MIT), o FTP foi desenvolvido para
  ser um método seguro e eficiente de compartilhamento de dados. Com a evolução
  da tecnologia e o aumento da capacidade de armazenamento, ele se consolidou
  como uma ferramenta indispensável para lidar com ativos digitais valiosos e
  informações sensíveis.
</p>

<h4>Funcionamento Técnico</h4>

<p>
  O FTP opera no modelo <strong>cliente-servidor</strong> e utiliza duas conexões
  distintas para garantir a eficiência e a organização do tráfego:
</p>

<ul>
  <li>
    <strong>Canal de Comando (Porta 21):</strong> Responsável pela troca de instruções
    e respostas entre o cliente e o servidor. É onde a comunicação logística acontece.
  </li>
  <li>
    <strong>Canal de Dados (Porta 20):</strong> Dedicado exclusivamente à transferência
    física dos arquivos.
  </li>
</ul>

<h4>Vantagens e Utilidades</h4>

<p>
  Embora seja essencial para a publicação de sites, o FTP é amplamente utilizado
  em outros setores que demandam tráfego de grandes volumes de informações:
</p>

<ul>
  <li>
    <strong>Transferência Simultânea:</strong> Permite enviar ou receber múltiplos
    arquivos ao mesmo tempo.
  </li>
  <li>
    <strong>Acesso Remoto:</strong> Possibilita baixar, editar ou gerenciar arquivos
    de qualquer lugar do mundo, desde que se tenha acesso e login.
  </li>
  <li>
    <strong>Gestão de Servidor:</strong> Oferece comandos para listar, renomear,
    mover e excluir pastas e documentos diretamente no servidor.
  </li>
  <li>
    <strong>Uso Multissetorial:</strong> Muito comum em gráficas (envio de artes
    pesadas) e produtoras de vídeo para o tráfego de arquivos brutos.
  </li>
</ul>

<h3>Conclusão: HTML e CSS</h3>

<p>
  A integração entre HTML e CSS é o que permite a gestão eficiente de sites
  modernos. Enquanto o HTML se ocupa da estrutura e do significado do conteúdo,
  o CSS assume a responsabilidade pela apresentação visual, permitindo
  alterações em larga escala com pouco esforço manual.
</p>

<h4>Estrutura de Marcação (HTML)</h4>

<p>
  O HTML organiza o conteúdo através de tags que indicam a função de cada
  elemento. Para títulos principais, utiliza-se a tag &lt;h1&gt;.
</p>

<ul>
  <li>
    <strong>Exemplo:</strong> &lt;h1&gt; Este é o título do texto &lt;/h1&gt;.
  </li>
</ul>

<h4>Estilização e Escalabilidade (CSS)</h4>

<p>
  Editar o HTML diretamente para alterar cores ou fontes é funcional em projetos
  pequenos, mas inviável em portais com centenas de páginas. O CSS resolve esse
  problema ao separar o conteúdo do design. As três formas de aplicação do CSS
  oferecem diferentes níveis de controle e organização:
</p>

<ul>
  <li>
    <strong>In-line:</strong> Aplicado diretamente na tag HTML. Útil para ajustes
    pontuais e rápidos.
  </li>
  <li>
    <strong>Interna:</strong> Definido dentro da tag &lt;style&gt; no cabeçalho do
    documento. Afeta apenas a página atual.
  </li>
  <li>
    <strong>Externa:</strong> As regras ficam em um arquivo separado (ex: estilo.css).
    É a forma mais profissional, pois um único arquivo pode controlar o visual de
    todo o site, garantindo unidade visual e facilidade de manutenção.
  </li>
</ul>

<h4>Benefícios Práticos</h4>

<p>O uso correto dessas linguagens proporciona:</p>

<ul>
  <li>
    <strong>Edição Massiva:</strong> Alterar uma única linha de código no CSS para
    mudar a cor de todos os títulos do site instantaneamente.
  </li>
  <li>
    <strong>Economia de Recursos:</strong> Redução do tamanho dos arquivos e do tempo
    de carregamento das páginas.
  </li>
  <li>
    <strong>Organização:</strong> Separação clara entre o que é informação (HTML)
    e o que é estética (CSS).
  </li>
</ul>
