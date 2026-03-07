<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Design de Interfaces: Fundamentos e Práticas</h2>

<Audios modulo="M10" aulas={["21", "22", "23", "24"]} />

<p>
  Nesta nova estapa, o foco recai sobre o design de interfaces (UI) e a
  experiência do usuário (UX), explorando ferramentas de prototipagem, técnicas
  de responsividade e acessibilidade. O objetivo é compreender como transformar
  a infraestrutura técnica em uma aplicação funcional, estética e eficiente para
  o usuário final.
</p>

<h4>Interface de Usuário (UI) vs. Experiência do Usuário (UX)</h4>

<p>
  A <strong>UI (User Interface)</strong> refere-se a toda a parte visual e interativa
  da aplicação. Envolve a criação e disposição de botões, ícones formulários e tipografia.
  Uma boa UI deve ser clara, consistente e adaptada ao público-alvo, garantindo que
  os elementos sejam facilmente clicáveis e legíveis, especialmente em dispositivos
  móveis.
</p>

<p>
  A <strong>UX (User Experience)</strong> foca na sensação e eficácia da interação
  do usuário com o sistema. O objetivo é tornar o uso simples e lógico, apresentando
  informações de forma organizada, prevenindo erros e orientando o usuário em caso
  de falhas. UI e UX são complementares: enquanto a UI cuida da aparência, a UX cuida
  da fluidez e da utilidade da jornada do usuário.
</p>

<h4>Boas Práticas de Design</h4>

<p>
  Para um design objetivo e otimizado, deve-se priorizar o uso estratégico de
  cores e a hierarquia visual. Exemplos práticos incluem a organização clara de
  produtos em sites de e-commerce ou a exibição direta de extratos em
  aplicativos bancários, facilitando a compreensão imediata dos dados
  apresentados.
</p>

<h3>Princípios de Design de Interface (Norman e Nielsen)</h3>

<p>
  O objetivo central do design de interface é proporcionar a melhor experiência
  ao usuário. Para orientar designers na criação de interfaces eficientes,
  existem diretrizes fundamentais conhecidas como
  <strong>princípios para um bom design</strong>.
</p>

<ul>
  <li>
    <strong>Design Visual (Feedback):</strong>
    O sistema deve fornecer retorno imediato sobre suas ações. O usuário precisa
    saber o que está acontecendo em tempo real, como uma barra de progresso durante
    um download ou uma confirmação de conclusão.
  </li>
  <li>
    <strong>Consistência:</strong>
    É a manutenção de padrões visuais e funcionais. Ícones, palavras e comportamentos
    devem ser os mesmos em todas as páginas para que o usuário não precise reaprender
    a usar o sistema a cada tela.
  </li>
  <li>
    <strong>Familiaridade:</strong>
    Utilização de símbolos, ícones e termos que já façam parte do cotidiano do usuário.
    Isso reduz o esforço cognitivo, pois os elementos são reconhecidos instantaneamente.
  </li>
  <li>
    <strong>Prevenção de Erros:</strong>
    O design deve ser projetado para evitar falhas do usuário. Isso inclui o uso
    de alertas em eventos críticos, como mensagens de confirmação antes de excluir
    um arquivo ou alterar dados importantes.
  </li>
  <li>
    <strong>Documentação e Suporte:</strong>
    O sistema deve oferecer ajuda acessível e manuais de utilização. A documentação
    serve para esclarecer dúvidas e permitir que o próprio usuário resolva problemas
    simples de forma autônoma.
  </li>
</ul>

<h4>Boas Práticas e o Processo de UX</h4>

<p>
  Para que uma plataforma seja eficaz, o design deve ser centrado no usuário e
  no nicho específico que a aplicação pretende atender. Antes de iniciar o
  visual, é fundamental entender as necessidades, comportamentos e dores de quem
  utilizará o sistema. Esse entendimento é estruturado através do processo de UX
  (User Experience). O processo de UX é dividido em etapas fundamentais:
</p>

<ul>
  <li>
    <strong>Pesquisa e descoberta:</strong> Fase de entendimento do público por meio
    de entrevistas e análise de concorrentes para identificar boas práticas e diferenciais.
  </li>
  <li>
    <strong>Definição e estruturação:</strong> Organização das informações coletadas
    para mapear o fluxo do usuário e criar esboços iniciais (wireframes) do layout.
  </li>
  <li>
    <strong>Design e prototipagem:</strong> Criação da interface visual (cores, ícones
    e marca) e de versões interativas. O protótipo serve para testar a navegação
    com o cliente antes de iniciar a programação.
  </li>
  <li>
    <strong>Implementação e testes:</strong> Transformação do protótipo em código
    funcional. Após o desenvolvimento, o sistema passa por testes de qualidade para
    garantir estabilidade e correção de funções.
  </li>
</ul>

<p>
  Além do fluxo de trabalho, o design moderno exige atenção à <strong
    >responsividade</strong
  >, garantindo que a interface se adapte a diferentes tamanhos de tela (do
  desktop ao smartphone), e à <strong>acessibilidade</strong>, assegurando que
  pessoas com deficiência consigam navegar e utilizar a plataforma sem
  barreiras.
</p>

<h4>Otimização de Performance de Interface Web</h4>

<p>
  A otimização de performance é o processo de melhorar a velocidade e a
  eficiência com que as páginas são carregadas e executadas. Sites rápidos
  aumentam a retenção de usuários, enquanto páginas lentas costumam causar
  abandono. Além disso, a otimização garante que a plataforma seja acessível
  mesmo para usuários com conexões de internet limitadas. As principais áreas
  para aplicar essa otimização são:
</p>

<ul>
  <li>
    <strong>Redução do tamanho de imagens:</strong> O uso de ferramentas para comprimir
    imagens sem perda significativa de qualidade evita que arquivos pesados comprometam
    a velocidade de carregamento.
  </li>
  <li>
    <strong>Minificação de arquivos:</strong> Consiste em remover espaços, quebras
    de linha e comentários desnecessários dos códigos CSS, HTML e JavaScript. Isso
    reduz o tamanho dos arquivos e acelera o processamento pelo navegador.
  </li>
  <li>
    <strong>Renderização e interatividade:</strong> Priorizar o carregamento apenas
    do CSS e dos recursos essenciais para a visualização inicial da página torna
    a aplicação mais leve e responsiva de imediato.
  </li>
  <li>
    <strong>Uso de Cache:</strong> Configurar cabeçalhos HTTP para que o navegador
    armazene recursos estáticos (que não mudam frequentemente). Isso permite que,
    em visitas futuras, o navegador carregue esses arquivos localmente, tornando
    o acesso muito mais rápido.
  </li>
</ul>

<h3>Introdução à Prototipagem com Figma</h3>

<p>
  O <strong>Figma</strong> é uma ferramenta de design colaborativo baseada na web,
  amplamente utilizada por designers de UI e UX para criar protótipos de interfaces.
  Ele pode ser acessado diretamente pelo navegador ou por uma versão desktop instalada
  no computador. A plataforma é intuitiva e permite a criação de versões interativas
  de um sistema antes do desenvolvimento real.
</p>

<h4>Primeiros Passos e Configurações de Tela</h4>

<p>
  O processo inicial no Figma envolve a criação de uma conta (com plano gratuito
  disponível) e a definição do espaço de trabalho. A estruturação do design
  segue alguns comandos fundamentais:
</p>

<ul>
  <li>
    <strong>Frames:</strong> São as áreas que representam o tamanho da tela (desktop,
    mobile, etc.). Ao selecionar a ferramenta "Frame", o Figma oferece modelos pré-programados
    no menu lateral direito.
  </li>
  <li>
    <strong>Edição de Bordas (Corner Radius):</strong> Permite arredondar os cantos
    da tela ou de elementos, conferindo um aspecto mais moderno ao design.
  </li>
  <li>
    <strong>Preenchimento (Fill):</strong> Ferramenta utilizada para definir as cores
    de fundo de telas, formas e componentes.
  </li>
</ul>

<h4>Manipulação de Elementos e Componentes</h4>

<p>
  A criação de elementos visuais é feita de forma direta através do menu de
  ferramentas, com ajustes detalhados no painel lateral direito:
</p>

<ul>
  <li>
    <strong>Texto:</strong> Ao inserir um texto, o menu lateral permite editar tipografia,
    tamanho, peso e cor da fonte.
  </li>
  <li>
    <strong>Criação de Botões:</strong> Uma técnica comum é digitar o texto, pressionar
    Esc e usar o atalho Shift + A (Auto Layout). Isso transforma o texto em um componente
    de botão, onde o fundo (Fill) pode ser colorido e o texto editado individualmente.
  </li>
  <li>
    <strong>Interatividade:</strong> O foco do Figma é permitir que o designer experimente
    e erre durante o processo de criação, facilitando a validação de ideias antes
    da implementação do código.
  </li>
</ul>

<h3>Conclusão: Design, Performance e Prototipagem</h3>

<p>
  Esta etapa consolidou o conhecimento sobre a criação de interfaces web, unindo
  fundamentos teóricos de design, técnicas de otimização técnica e a prática
  inicial de prototipagem.
</p>

<h4>Princípios Essenciais do Design</h4>

<p>
  O foco é proporcionar a melhor experiência ao usuário através de diretrizes
  claras:
</p>

<ul>
  <li>
    <strong>Design Visual (Feedback):</strong> Informar ao usuário o que está acontecendo
    no sistema em tempo real.
  </li>
  <li>
    <strong>Consistência:</strong> Manter padrões de ícones, palavras e comportamentos
    em todas as páginas.
  </li>
  <li>
    <strong>Familiaridade:</strong> Usar símbolos e termos fáceis de reconhecer pelo
    público.
  </li>
  <li>
    <strong>Prevenção de Erros:</strong> Criar mecanismos que evitem ações indesejadas
    (como alertas de confirmação).
  </li>
  <li>
    <strong>Documentação e Suporte:</strong> Oferecer ajuda acessível e manuais de
    utilização.
  </li>
</ul>

<h4>Otimização de Performance</h4>

<p>
  A performance é crucial para a retenção do usuário e acessibilidade. As
  melhorias focam na velocidade de carregamento e execução através de:
</p>

<ul>
  <li>Redução do tamanho de imagens.</li>
  <li>Minificação de arquivos (CSS, HTML e JavaScript).</li>
  <li>Renderização eficiente de recursos essenciais.</li>
  <li>Uso de cache do navegador para recursos estáticos.</li>
</ul>

<h4>Prática em Prototipagem (Figma)</h4>

<p>
  A introdução à ferramenta permitiu a criação de um projeto inicial, explorando
  as seguintes funcionalidades básicas:
</p>

<ul>
  <li>Configuração de <strong>Frames</strong> (tamanhos de tela).</li>
  <li>
    Personalização visual com <strong>Fill</strong> (cores de fundo) e
    <strong>Corner Radius</strong> (bordas arredondadas).
  </li>
  <li>
    Manipulação de <strong>Textos</strong> e suas propriedades no menu lateral.
  </li>
  <li>
    Criação de <strong>Botões</strong> funcionais utilizando o atalho Shift + A (Auto
    Layout).
  </li>
</ul>
