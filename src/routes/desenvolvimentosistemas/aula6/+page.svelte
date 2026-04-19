<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Estrutura e Modelagem de Sistemas</h2>

<Audios modulo="M12" aulas={["21", "22", "23", "24"]} />

<p>
  A modelagem de sistemas utiliza <strong>modelos gráficos e diagramas</strong> para
  facilitar a visualização da totalidade do software. Enquanto listas de texto descrevem
  etapas, o modelo gráfico permite analisar as relações entre diferentes objetos
  e funções, ajudando a identificar falhas e oportunidades de melhoria na lógica
  do sistema antes da codificação. Essa abordagem busca compreender o todo e suas
  conexões, validando a lógica dos dados e encontrando caminhos mais eficientes para
  o tráfego de informações.
</p>

<h3>Análise Orientada a Objetos (OO)</h3>

<p>
  A análise orientada a objetos organiza o sistema em torno de <strong
    >objetos</strong
  >, que são unidades de dados com estrutura e operações próprias. Os principais
  conceitos dessa análise são:
</p>

<ul>
  <li>
    <strong>Objetos:</strong> Elementos que possuem atributos (dados) e métodos (comportamentos).
    Eles trocam mensagens entre si para executar ações.
  </li>
  <li>
    <strong>Classes:</strong> Agrupamentos de objetos que compartilham a mesma interface
    e respondem às mesmas mensagens. A classe é o "molde" ou a especificação para
    a criação de objetos.
  </li>
  <li>
    <strong>Atributos:</strong> Informações e características que descrevem o objeto.
  </li>
  <li>
    <strong>Métodos (Operações):</strong> Funções ou procedimentos que alteram ou
    manipulam os dados do objeto.
  </li>
  <li>
    <strong>Encapsulamento:</strong> Técnica que restringe o acesso aos atributos
    de uma classe, permitindo que sejam acessados apenas por seus próprios métodos.
  </li>
  <li>
    <strong>Herança:</strong> Mecanismo que permite que uma subclasse herde propriedades
    e comportamentos de uma superclasse, podendo adicionar novas características.
  </li>
</ul>

<h4>UML (Unified Modeling Language)</h4>

<p>
  A UML é uma linguagem de notação padrão e visual, utilizada para especificar,
  construir e documentar artefatos de sistemas complexos. Ela não é uma
  linguagem de programação, mas sim uma ferramenta independente que padroniza a
  comunicação entre desenvolvedores.
</p>

<ul>
  <li>
    <strong>Independência:</strong> A UML pode ser aplicada independentemente da
    linguagem de programação escolhida para o projeto.
  </li>
  <li>
    <strong>Visualização:</strong> Utiliza diagramas para identificar funções, limites
    do sistema e o comportamento dos objetos.
  </li>
  <li>
    <strong>Artefatos:</strong> Todos os documentos gerados a partir da UML são chamados
    de artefatos.
  </li>
  <li>
    <strong>Diferenciação:</strong> Sistemas orientados a objetos utilizam UML; sistemas
    procedurais costumam utilizar fluxogramas.
  </li>
</ul>

<h4>Ferramentas CASE e Diagramas</h4>

<p>
  A modelagem em UML é operacionalizada através de diversos diagramas que
  capturam diferentes perspectivas do sistema, como:
</p>

<ul>
  <li>
    <strong>Casos de Uso:</strong> Descrevem as funcionalidades e as interações do
    sistema com atores externos.
  </li>
  <li>
    <strong>Diagramas de Sequência:</strong> Mostram a ordem temporal das trocas
    de mensagens entre objetos.
  </li>
  <li>
    <strong>Diagramas de Estados:</strong> Representam as mudanças de comportamento
    de um objeto em resposta a eventos.
  </li>
</ul>

<h3>Ferramentas CASE (Computer-Aided Software Engineering)</h3>

<p>
  As ferramentas <strong>CASE</strong> são softwares criados para auxiliar no desenvolvimento
  de outros softwares. Elas fornecem suporte automatizado para processos, métodos
  e atividades, visando aumentar a qualidade do produto final, reduzir riscos e garantir
  a segurança da aplicação, especialmente em projetos de alta complexidade.
</p>

<h4>Classificação das Ferramentas</h4>

<p>
  As ferramentas CASE podem ser categorizadas de acordo com sua abrangência no
  ciclo de vida do projeto:
</p>

<ul>
  <li>
    <strong>Horizontais:</strong> Oferecem serviços utilizados durante
    <strong>todo</strong> o processo de desenvolvimento (ex: ferramentas de documentação
    ou gerenciamento de projetos).
  </li>
  <li>
    <strong>Verticais:</strong> São focadas em
    <strong>fases específicas</strong> e pontuais do desenvolvimento (ex: um gerador
    de código ou uma ferramenta de design de interface).
  </li>
</ul>

<h4>Serviços e Funcionalidades</h4>

<p>Essas ferramentas automatizam diversas atividades críticas, tais como:</p>

<ul>
  <li>Planejamento e Gerenciamento de Projetos.</li>
  <li>Levantamento e Análise de Requisitos.</li>
  <li>Projeto de Arquitetura e Interfaces.</li>
  <li>Programação e Gerenciamento de Configuração.</li>
  <li>Controle de Qualidade e Testes.</li>
</ul>

<h4>Arquitetura e Requisitos das Ferramentas CASE</h4>

<p>
  Como o usuário de uma ferramenta CASE é o próprio desenvolvedor, a definição
  de seus requisitos é complexa e envolve análise de mercado e comparação com
  softwares similares. A arquitetura dessas ferramentas geralmente segue um
  modelo <strong>modular baseado em componentes</strong>, o que garante
  flexibilidade. Os principais pontos de sua arquitetura incluem:
</p>

<ul>
  <li>
    <strong>Repositório de dados:</strong> Onde as informações do projeto são centralizadas.
  </li>
  <li>
    <strong>Mecanismos de interação:</strong> Como a ferramenta troca informações
    com outros softwares.
  </li>
  <li>
    <strong>Modularidade:</strong> Facilita a configuração para diferentes tipos
    de uso e plataformas.
  </li>
</ul>

<h4>Processo de Seleção</h4>

<p>
  A escolha de uma ferramenta CASE deve ser criteriosa e baseada em uma
  comparação técnica de dados. O processo envolve:
</p>

<ol>
  <li>
    <strong>Definição do propósito:</strong> Para que a ferramenta será usada?
  </li>
  <li>
    <strong>Estabelecimento do escopo:</strong> Identificação de restrições e suposições.
  </li>
  <li>
    <strong>Avaliação:</strong> Teste das ferramentas propostas em relação aos critérios
    do projeto.
  </li>
  <li>
    <strong>Análise de resultados:</strong> Comparação das funcionalidades e custos
    para a tomada de decisão final.
  </li>
</ol>

<h3>Diagrama de Casos de Uso</h3>

<p>
  O <strong>Diagrama de Casos de Uso</strong> é uma ferramenta da UML que
  descreve as funcionalidades de um sistema sob a perspectiva de um observador
  externo. Ele foca no <strong>o que</strong> o sistema faz, e não no como, sendo
  essencial para documentar requisitos e dividir o desenvolvimento em tarefas gerenciáveis.
</p>

<h4>Componentes Principais</h4>

<p>O diagrama utiliza uma simbologia simples para representar as interações:</p>

<ul>
  <li>
    <strong>Atores:</strong> Representados por "bonecos de palito", simbolizam os
    usuários humanos ou sistemas externos que interagem com o software.
  </li>
  <li>
    <strong>Caso de Uso:</strong> Representado por elipses (balões), contém um verbo
    e um substantivo que identificam uma funcionalidade ou tarefa específica (ex:
    "Realizar Login", "Gerar Relatório").
  </li>
  <li>
    <strong>Associação:</strong> Linhas que conectam atores aos casos de uso, indicando
    que há uma interação entre eles.
  </li>
</ul>

<h4>Relacionamentos entre Casos de Uso</h4>

<p>
  Existem formas de conectar os casos de uso para evitar repetições e detalhar
  comportamentos específicos:
</p>

<ul>
  <li>
    <strong>Include (Inclusão):</strong> Indica uma execução obrigatória. Se o Caso
    A inclui o Caso B, sempre que A for executado, B também será (ex: "Finalizar
    Compra" inclui "Validar Cartão").
  </li>
  <li>
    <strong>Extend (Extensão):</strong> Indica uma execução opcional ou condicional.
    O Caso B pode ser executado após o Caso A, mas apenas em situações específicas
    (ex: "Realizar Pedido" pode ser estendido por "Aplicar Cupom de Desconto").
  </li>
  <li>
    <strong>Generalization (Generalização/Herança):</strong> Indica que um caso de
    uso é uma especialização de outro. O caso filho herda o comportamento do caso
    pai, mas pode ter detalhes próprios (ex: "Realizar Pagamento" é o pai, enquanto
    "Pagar com Boleto" e "Pagar com Cartão" são os filhos).
  </li>
</ul>

<p>
  O uso correto desses elementos permite visualizar claramente os limites do
  sistema e as responsabilidades de cada usuário.
</p>

<h3>Diagrama de Classe</h3>

<p>
  O Diagrama de Classe é um modelo estático da UML que descreve a estrutura de
  um sistema ao exibir suas classes, atributos, operações (métodos) e os
  relacionamentos entre os objetos. Ele serve como o mapa principal para a
  construção do código, detalhando como as entidades do software "se conhecem" e
  interagem.
</p>

<h4>Estrutura de uma Classe</h4>

<p>Cada classe é representada por um retângulo dividido em três partes:</p>

<ol>
  <li><strong>Nome da Classe:</strong> Identificação do objeto.</li>
  <li>
    <strong>Atributos:</strong> Dados e propriedades. Podem incluir tipo e valor
    inicial.
  </li>
  <li>
    <strong>Operações (Métodos):</strong> Funções e comportamentos que a classe executa.
  </li>
</ol>

<p>A visibilidade dos atributos e métodos é indicada por símbolos:</p>

<ul>
  <li><strong>+ Público:</strong> Acessível por qualquer outra classe.</li>
  <li>
    <strong># Protegido:</strong> Acessível apenas pela própria classe e suas subclasses
    (herança).
  </li>
  <li>
    <strong>- Privado:</strong> Acessível apenas pela própria classe (encapsulamento).
  </li>
</ul>

<h4>Relacionamentos no Diagrama</h4>

<p>
  As linhas de ligação entre as classes definem como elas dependem uma da outra:
</p>

<ul>
  <li>
    <strong>Associação:</strong> Conexão simples onde objetos de uma classe estão
    ligados a objetos de outra.
  </li>
  <li>
    <strong>Generalização (Herança):</strong> Uma classe filha herda propriedades
    e métodos de uma classe pai (elemento geral).
  </li>
  <li>
    <strong>Dependência:</strong> Indica que uma classe utiliza serviços ou recursos
    de outra para funcionar.
  </li>
  <li>
    <strong>Agregação Regular:</strong> Relacionamento "todo-parte", onde a "parte"
    pode existir independentemente do "todo".
  </li>
  <li>
    <strong>Composição:</strong> Uma forma estrita de agregação onde a "parte" não
    existe sem o "todo" (se o todo for excluído, as partes também são).
  </li>
</ul>

<h4>Importância</h4>

<p>
  Este diagrama é fundamental para a análise orientada a objetos, pois traduz
  visualmente as funcionalidades do sistema em uma estrutura lógica que pode ser
  diretamente mapeada para linguagens de programação como Java, C++ ou Python.
</p>

<h3>Diagramas de Sequência e de Estados</h3>

<p>
  Enquanto os diagramas de classe focam na estrutura parada do sistema, os
  diagramas de <strong>Sequência</strong> e de <strong>Estados</strong> focam no
  comportamento dinâmico, ou seja, em como as coisas acontecem e mudam ao longo do
  tempo.
</p>

<h4>Diagrama de Sequência</h4>

<p>
  O <strong>Diagrama de Sequência</strong> descreve como os objetos interagem entre
  si, focando na ordem temporal das trocas de mensagens. Ele é fundamental para visualizar
  o passo a passo de uma funcionalidade específica.
</p>

<ul>
  <li>
    <strong>Objetos:</strong> Representados no topo do diagrama, cada um possui uma
    "linha de vida" (vertical) que indica sua existência durante a interação.
  </li>
  <li>
    <strong>Mensagens:</strong> Setas horizontais que ligam as linhas de vida, representando
    a comunicação entre os objetos
  </li>
  <li>
    <strong>Tipos de Mensagens:</strong>
    <ul>
      <li>
        <strong>Síncronas (Procedurais):</strong> O remetente espera por uma resposta
        antes de prosseguir (aninhamento).
      </li>
      <li>
        <strong>Assíncronas (Planas):</strong> O remetente envia a mensagem e continua
        sua execução sem esperar resposta imediata.
      </li>
    </ul>
  </li>
</ul>

<h4>Diagrama de Estados</h4>

<p>
  O <strong>Diagrama de Estados</strong> (ou Máquina de Estados) modela o ciclo de
  vida de um único objeto, mostrando as diferentes condições (estados) pelas quais
  ele passa em resposta a eventos externos ou internos.
</p>

<ul>
  <li>
    <strong>Estado:</strong> Representa uma condição ou situação na vida de um objeto
    (ex: um pedido pode estar nos estados "Pendente", "Pago" ou "Cancelado").
  </li>
  <li>
    <strong>Transição:</strong> Setas que indicam a mudança de um estado para outro,
    geralmente disparadas por um evento.
  </li>
  <li>
    <strong>Componentes de Fluxo:</strong>
    <ul>
      <li>
        <strong>Estado Inicial:</strong> O ponto de partida do objeto (círculo preenchido).
      </li>
      <li>
        <strong>Estados Intermediários:</strong> As diversas fases que o objeto percorre.
      </li>
      <li>
        <strong>Estado Final:</strong> O encerramento do ciclo de vida do objeto
        (círculo com borda).
      </li>
    </ul>
  </li>
</ul>

<h4>Diferença Essencial</h4>

<ul>
  <li>
    <strong>Sequência:</strong> Foca na <strong>troca de mensagens</strong> entre
    vários objetos para realizar uma tarefa.
  </li>
  <li>
    <strong>Estados:</strong> Foca na <strong>mudança de comportamento</strong> e
    condição de um único objeto.
  </li>
</ul>

<h3>Conclusão: Modelagem e Análise Orientada a Objetos</h3>

<p>
  Esta etapa finaliza o entendimento sobre como estruturar visualmente um
  software antes de sua construção. A <strong
    >Análise Orientada a Objetos</strong
  >
  fornece a base lógica, enquanto a <strong>UML</strong> oferece a padronização visual
  necessária para que equipes de desenvolvimento compreendam o sistema de forma unificada
  e eficiente.
</p>

<ul>
  <li>
    <strong>Fundamentos da OO:</strong> O foco na criação de componentes reutilizáveis
    (objetos e classes) que organizam dados (atributos) e comportamentos (métodos)
    de forma clara.
  </li>
  <li>
    <strong>Padronização com UML:</strong> O uso de uma linguagem visual independente
    de programação para documentar, especificar e construir sistemas complexos.
  </li>
  <li>
    <strong>Diversidade de Diagramas:</strong>
    <ul>
      <li>
        <strong>Casos de Uso:</strong> O que o sistema faz (visão externa).
      </li>
      <li>
        <strong>Classes:</strong> Como o sistema é estruturado (visão estática).
      </li>
      <li>
        <strong>Sequência:</strong> Como os componentes interagem no tempo (visão
        dinâmica).
      </li>
      <li>
        <strong>Estados:</strong> Como um objeto muda de condição (visão de comportamento).
      </li>
    </ul>
  </li>
  <li>
    <strong>Apoio Tecnológico:</strong> O uso de ferramentas CASE para automatizar
    a criação desses diagramas e gerenciar o ciclo de vida do software com maior
    segurança e menor risco de falhas.
  </li>
</ul>

<h4>Dicas para Internalização e Estudo</h4>

<ul>
  <li>
    <strong>Pratique a Visualização:</strong> Tente converter processos simples do
    dia a dia (como sacar dinheiro em um caixa eletrônico) em um Diagrama de Casos
    de Uso ou de Sequência.
  </li>
  <li>
    <strong>Consulte Padrões:</strong> Use a UML como um dicionário; não é preciso
    decorar tudo, mas sim saber consultar as notações (símbolos e linhas) para interpretar
    corretamente os artefatos de um projeto.
  </li>
  <li>
    <strong>Aplicação Prática:</strong> O conhecimento de modelagem é o que diferencia
    um programador de um engenheiro de software. O primeiro escreve código; o segundo
    projeta soluções sustentáveis.
  </li>
</ul>
