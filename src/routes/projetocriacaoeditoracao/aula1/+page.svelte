<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Fundamentos do Projeto Web</h2>

<Audios modulo="M5" aulas={["01", "02", "03", "04"]} />

<p>
  O objetivo central de um website é <strong>informar</strong>. Embora a
  estética seja relevante, a prioridade deve ser a funcionalidade, a facilidade
  de manuseio e a experiência do usuário. Um site eficiente é aquele que
  demonstra ter sido planejado especificamente para quem o utiliza.
</p>

<p>
  O ponto de partida para um bom projeto é o <strong>briefing</strong>. Este
  documento define as diretrizes do sistema, estabelecendo claramente o que o
  site deve e o que não pode fazer. É no briefing que se determina a finalidade
  do projeto, o que ditará as prioridades do desenvolvimento.
</p>

<h3>Tipos de Projetos e Prioridades</h3>

<ul>
  <li>
    <strong>Intranet:</strong> O foco é a acessibilidade. As informações mais utilizadas
    pela empresa devem estar ao alcance rápido, sendo o layout um fator secundário.
  </li>
  <li>
    <strong>Site Institucional:</strong> Deve focar no visual e na imagem da empresa.
    O layout precisa cativar o visitante e transmitir credibilidade, contendo o máximo
    de informações relevantes sobre a organização.
  </li>
  <li>
    <strong>Site de Vendas (E-commerce):</strong> A prioridade é o produto. Os elementos
    cruciais para o usuário são, nesta ordem: preço, informações detalhadas do produto
    e confiabilidade da loja.
  </li>
  <li>
    <strong>Site de Notícias:</strong> O foco reside na atualidade e na navegabilidade.
    As notícias mais recentes devem aparecer primeiro, com links que permitam ao
    leitor aprofundar-se no conteúdo.
  </li>
</ul>

<h3>O Mapa Mental no Projeto Web</h3>

<p>
  O <strong>mapa mental</strong> funciona como o esqueleto ou a fundação do site.
  Ele deve ser elaborado após a coleta de informações (briefing e personas) e antes
  da execução técnica. Sua função é definir a hierarquia do conteúdo, estabelecendo
  o que é principal e o que é secundário. Investir tempo nesta etapa evita o retrabalho,
  que é uma das maiores fontes de frustração em um projeto.
</p>

<p>
  A construção dessa estrutura pode ser feita de forma analógica (papel) ou
  digital, desde que seja bem executada. O mapa mental permite visualizar como o
  projeto se "sustenta" antes mesmo de começar a ser construído visualmente.
</p>

<h4>Princípios de Construção e Hierarquia</h4>

<ul>
  <li>
    <strong>Do Geral para o Específico:</strong> O planejamento deve começar pelas
    informações que todos os usuários precisam acessar (genéricas) e avançar até
    as informações de nicho (específicas).
  </li>
  <li>
    <strong>Fundações do Projeto:</strong> O mapa mental é a base que sustenta o
    site; sem ele, a organização se perde durante o desenvolvimento.
  </li>
  <li>
    <strong>Hierarquia de Conteúdo:</strong> É a definição clara de prioridades,
    baseada em conceitos de usabilidade que determinam a facilidade de navegação
    do usuário.
  </li>
  <li>
    <strong>Expansão:</strong> Uma vez definido o esqueleto, o próximo passo é preencher
    cada seção com as informações detalhadas e o conteúdo final.
  </li>
</ul>

<h3>Mapa Mental Digital</h3>

<p>
  Embora o papel seja funcional, o uso de softwares especializados para mapas
  mentais é mais eficiente por permitir correções e ajustes sem "sujeira" ou
  rasuras. Existem diversas opções no mercado, tanto gratuitas (Free Mind, Free
  Plane, Coggle) quanto pagas (Mind Manager, Mind Meister, Xmind), sendo a
  escolha da ferramenta menos importante do que a habilidade de utilizá-la.
</p>

<p>
  A versão digital facilita a visualização da estrutura antes da execução,
  permitindo que a equipe de desenvolvimento, clientes e patrocinadores
  compreendam a hierarquia e o fluxo de navegação. É o momento ideal para
  definir o que está ligado a quê, quais caminhos o usuário percorrerá e quais
  são os limites de profundidade do conteúdo do site.
</p>

<h4>Vantagens e Segurança no Projeto</h4>

<ul>
  <li>
    <strong>Flexibilidade:</strong> Permite acrescentar, remover e realocar páginas
    ou seções com facilidade.
  </li>
  <li>
    <strong>Prevenção de Retrabalho:</strong> Facilita a discussão e aprovação da
    estrutura com o cliente antes de iniciar a programação ou o design.
  </li>
  <li>
    <strong>Alinhamento de Expectativas:</strong> Evita mudanças estruturais tardias
    que exigiriam refazer todo o projeto.
  </li>
  <li>
    <strong>Documentação e Segurança:</strong> Manter o mapa mental arquivado e assinado
    pelos envolvidos serve como garantia profissional; qualquer alteração estrutural
    após a aprovação justifica novos prazos ou custos.
  </li>
</ul>

<h3>Responsividade e Mobile First</h3>

<p>
  Atualmente, o número de conexões via dispositivos móveis supera a população
  mundial, tornando a <strong>responsividade</strong> obrigatória. Um site responsivo
  é aquele que adapta sua interface para ser visualizado de forma eficiente em telas
  menores, garantindo que a experiência do usuário não seja prejudicada pela limitação
  de espaço.
</p>

<p>
  O design para smartphones exige um equilíbrio entre o espaço escasso e a
  ergonomia. Como as telas são pequenas, mas a interação é feita com os dedos,
  os elementos clicáveis devem ser grandes e fáceis de acionar, sem desperdiçar
  áreas úteis. O foco absoluto deve ser o <strong>conteúdo</strong>,
  simplificando a interface ao máximo.
</p>

<h4>Estratégias para um Bom Layout Mobile</h4>

<ul>
  <li>
    <strong>Hierarquia de Informação:</strong> Utilize a lógica da pirâmide invertida,
    apresentando o conteúdo mais importante e geral logo no início, deixando os detalhes
    para o final da página.
  </li>
  <li>
    <strong>Layout Verticalizado:</strong> O site deve ser planejado para o uso com
    o celular em pé. A orientação horizontal deve ser evitada, exceto em casos específicos
    de consumo de vídeo.
  </li>
  <li>
    <strong>Design Limpo:</strong> Prefira fundos neutros (branco ou preto) e evite
    o excesso de cores ou elementos visuais que poluam a tela.
  </li>
  <li>
    <strong>Botões vs. Links:</strong> Substitua links sublinhados por botões visíveis,
    que facilitam o clique em telas sensíveis ao toque.
  </li>
  <li>
    <strong>Call-to-Action (CTA):</strong> Utilize "chamadas para ação" (como "Saiba
    mais" ou "Compre agora") como atalhos para que o usuário realize rapidamente
    o objetivo principal do site.
  </li>
</ul>

<h3>Domínio e Hospedagem</h3>

<p>
  Antes de publicar um site, é necessário definir o seu nome (<strong
    >domínio</strong
  >) e o local onde ele ficará armazenado (<strong>hospedagem</strong>). Embora
  muitas empresas ofereçam ambos os serviços em conjunto, são conceitos
  distintos: o domínio é o endereço (a identidade governamental), enquanto a
  hospedagem é o servidor que mantém os arquivos online.
</p>

<h4>Escolha do Domínio</h4>

<p>
  A escolha do nome deve ser estratégica e considerar a facilidade de digitação
  e memorização. Como o acesso via dispositivos móveis é predominante, o domínio
  deve ser amigável para teclados de smartphones e corretores ortográficos.
</p>

<ul>
  <li>
    <strong>Simplicidade:</strong> Evite nomes longos, hifens ou letras duplicadas
    que gerem confusão na fala ou escrita.
  </li>
  <li>
    <strong>Acessibilidade:</strong> Fuja de letras pouco comuns (W, K, Y) e nomes
    complexos que dificultem a digitação em celulares.
  </li>
  <li>
    <strong>Aspecto Jurídico:</strong> Não utilize marcas registradas de terceiros
    para evitar problemas legais.
  </li>
  <li>
    <strong>Coerência Geográfica:</strong> Use extensões adequadas. O ".br" é indicado
    para empresas brasileiras, enquanto extensões regionais (ex: ".sp.gov.br") podem
    limitar a percepção de alcance da marca.
  </li>
</ul>

<h4>Registro e Implementação</h4>

<p>
  No Brasil, o registro de domínios com final ".br" é coordenado pelo <strong
    >NIC.br</strong
  >
  através do site <strong>registro.br</strong>. O processo envolve verificar a
  disponibilidade do nome, fornecer dados como CPF ou CNPJ e realizar o
  pagamento de renovação anual.
</p>

<ul>
  <li>
    <strong>Disponibilidade:</strong> Caso o nome desejado já exista, o sistema sugere
    alternativas próximas.
  </li>
  <li>
    <strong>Hospedagem:</strong> Após garantir o domínio, deve-se contratar um servidor.
    A escolha deve ser baseada em pesquisa de mercado, avaliando pontos como espaço
    de armazenamento, funcionalidades extras, suporte técnico e custo-benefício para
    o tipo de projeto.
  </li>
</ul>

<h3>Conclusão</h3>

<p>
  Este módulo consolidou os pilares fundamentais para o desenvolvimento de
  projetos web, enfatizando que a funcionalidade e a entrega de informação ao
  usuário são as prioridades máximas. A estruturação correta, desde a concepção
  até a publicação, garante a viabilidade técnica e o sucesso comercial do site.
</p>
