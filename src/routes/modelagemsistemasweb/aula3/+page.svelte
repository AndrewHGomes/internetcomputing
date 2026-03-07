<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Engenharia de Requisitos</h2>

<Audios modulo="M8" aulas={["09", "10", "11", "12"]} />

<p>
  A construção de um software é um processo planejado que traduz as necessidades
  de negócio em soluções técnicas. O coração desse planejamento é a <strong>
    Engenharia de Requisitos
  </strong>, que identifica o que o sistema deve fazer para satisfazer o
  usuário. Os requisitos são a base que guia todas as atividades do projeto,
  conectando o fluxo do processo de negócio ao código final.
</p>

<p>
  Um requisito mal interpretado resulta em um software que executa tarefas
  diferentes das esperadas, gerando retrabalho e custos. Por isso, a coleta e a
  descrição dos requisitos devem ser feitas em linguagem clara para que tanto o
  cliente quanto a equipe técnica compartilhem o mesmo entendimento sobre o
  funcionamento do sistema.
</p>

<h4>O Processo de Entendimento de Requisitos</h4>

<p>
  O levantamento de requisitos é organizado em quatro etapas fundamentais para
  garantir a qualidade do projeto:
</p>

<ul>
  <li>
    <strong>Estudo de Viabilidade:</strong> Analisa se o software pode ser construído
    considerando limitações técnicas, prazos e recursos financeiros. É a primeira
    validação antes do investimento de tempo e esforço.
  </li>
  <li>
    <strong>Coleta de Requisitos:</strong> Fase de entrevistas e reuniões com usuários
    e clientes para identificar suas necessidades e ideias sobre o que o sistema
    deve realizar.
  </li>
  <li>
    <strong>Especificação de Requisitos:</strong> Momento de documentar e detalhar
    cada funcionalidade de forma escrita, clara e direta, transformando o que foi
    falado em um registro formal.
  </li>
  <li>
    <strong>Validação de Requisitos:</strong> Revisão final junto ao usuário para
    garantir que o que foi documentado está correto e reflete fielmente as regras
    de negócio.
  </li>
</ul>

<h4>Importância do Detalhamento</h4>

<p>
  Quanto mais complexo o sistema (como o controle de uma indústria química),
  maior a necessidade de decompor os requisitos em etapas menores e mais
  gerenciáveis. Isso permite entender as dependências entre dados e a ordem
  correta de execução das funcionalidades, garantindo que o software final seja
  robusto e eficiente.
</p>

<h3>Ciclo de Vida da Engenharia de Requisitos</h3>

<p>
  A Engenharia de Requisitos opera através de um ciclo de vida evolutivo e
  complementar, onde cada etapa refina o entendimento do que o software deve
  realizar. Este processo detalha a jornada desde a ideia inicial até a
  manutenção das funcionalidades ao longo do tempo.
</p>

<h4>Etapas do Ciclo de Vida</h4>

<ul>
  <li>
    <strong>Concepção:</strong> É o ponto de partida para entender o problema e o
    cenário do cliente. Estabelece a comunicação inicial entre as equipes técnica
    e de negócio, focando no objetivo macro do projeto.
  </li>
  <li>
    <strong>Levantamento:</strong> Fase de imersão detalhada por meio de entrevistas
    com usuários. Utiliza-se a modelagem de processos de negócio para identificar
    cada funcionalidade que o software deve possuir.
  </li>
  <li>
    <strong>Elaboração:</strong> Refinamento das informações coletadas. Aqui, os
    requisitos são expandidos para modelos técnicos, definindo cenários de uso e
    avaliando as restrições do sistema.
  </li>
  <li>
    <strong>Negociação:</strong> Momento de conciliação entre analistas e clientes.
    Priorizam-se os requisitos que agregam mais valor ao negócio, ajustando expectativas
    de custo, prazo e escopo.
  </li>
  <li>
    <strong>Especificação:</strong> Tradução dos requisitos negociados em modelos
    de implementação. Define-se a "receita" do software: tecnologias, linguagens
    de programação, banco de dados e a arquitetura técnica.
  </li>
  <li>
    <strong>Validação:</strong> Revisão técnica e gerencial para garantir que a especificação
    esteja clara, coerente e sem erros de comunicação. Confirma-se se os requisitos
    atendem fielmente aos processos da empresa.
  </li>
  <li>
    <strong>Gestão de Requisitos:</strong> Atividades contínuas de controle, rastreamento
    e modificação. É essencial para lidar com mudanças que surgem devido a novas
    necessidades de mercado ou de negócio durante ou após o desenvolvimento.
  </li>
</ul>

<h4>Resumo da Essência</h4>

<p>
  Os requisitos são o alicerce do projeto. Para que o software tenha sucesso,
  eles precisam ser:
</p>

<ol>
  <li>
    <strong>Completos:</strong> Não deixar lacunas sobre o que deve ser feito.
  </li>
  <li>
    <strong>Claros:</strong> Evitar ambiguidades que levem a erros de codificação.
  </li>
  <li>
    <strong>Coerentes:</strong> Não apresentar contradições entre diferentes funcionalidades.
  </li>
</ol>

<h3>Documento de Especificação de Requisitos</h3>

<p>
  O <strong>Documento de Especificação de Requisitos</strong> funciona como uma descrição
  macro e formal de todas as funcionalidades que devem compor o sistema. Ele serve
  como o alicerce para definir o escopo do projeto, garantindo que nenhum item essencial
  seja esquecido antes do início do detalhamento técnico.
</p>

<p>
  Este documento lista os requisitos <strong>suficientes e necessários</strong>,
  servindo como um guia para que o desenvolvedor tenha uma compreensão clara do
  produto final. Ele não foca no "como" a funcionalidade funciona internamente,
  mas sim no "o que" deve existir no software. Essa clareza é mantida através de
  comunicação contínua entre a equipe e o cliente até a entrega do sistema.
</p>

<h4>Características do Documento</h4>

<ul>
  <li>
    <strong>Visão Macro:</strong> Lista as funcionalidades sem entrar em detalhes
    técnicos de execução.
  </li>
  <li>
    <strong>Definição de Escopo:</strong> Garante que todos os requisitos que precisam
    de detalhamento futuro (como Casos de Uso) foram devidamente identificados.
  </li>
  <li>
    <strong>Base para Classificação:</strong> É a partir deste documento que os requisitos
    são divididos em funcionais e não funcionais.
  </li>
</ul>

<h4>Exemplo Prático: E-commerce de Roupas</h4>

<p>
  Em um documento de especificação para um site de vendas, a lista de requisitos
  incluiria:
</p>

<ul>
  <li>Cadastro de Produtos.</li>
  <li>Cadastro de Clientes.</li>
  <li>Catálogo de Produtos.</li>
  <li>Carrinho de Compras.</li>
  <li>Formas de Pagamento.</li>
  <li>Cálculo de Frete.</li>
</ul>

<h3>Requisitos Funcionais e Não Funcionais</h3>

<p>
  Os requisitos representam as necessidades, objetivos, propriedades e
  restrições que um sistema deve apresentar para satisfazer os usuários e
  cumprir padrões técnicos. Eles são as condições necessárias para atingir um
  objetivo específico dentro de um software, indo além de simples funções e
  abrangendo também o comportamento esperado do sistema.
</p>

<h4>Requisitos Funcionais (RF)</h4>

<p>
  Os <strong>Requisitos Funcionais (RF)</strong> descrevem
  <strong>o que</strong> o software faz, ou seja, as tarefas, serviços e funcionalidades
  que o sistema deve executar. Eles tratam do processamento de dados, cálculos, entradas,
  saídas e mudanças de estado do sistema conforme a interação do usuário.
</p>

<ul>
  <li><strong>Foco:</strong> Funcionalidades e serviços do sistema.</li>
  <li>
    <strong>Exemplos:</strong>
    <ul>
      <li>Cadastrar profissionais ou clientes (Entrada).</li>
      <li>Emitir relatórios de vendas (Saída).</li>
      <li>Consultar dados pessoais.</li>
      <li>
        Alterar o status de um atendimento de "em espera" para "concluído".
      </li>
    </ul>
  </li>
</ul>

<h4>Requisitos Não Funcionais (RNF)</h4>

<p>
  Os <strong>Requisitos Não Funcionais (RNF)</strong> descrevem
  <strong>como</strong> o software deve ser em termos de qualidade e restrições.
  Eles dão suporte aos requisitos funcionais, impondo critérios como tempo de resposta,
  padrões de segurança, linguagem de programação ou normas específicas da organização.
</p>

<ul>
  <li>
    <strong>Foco:</strong> Desempenho, usabilidade, confiabilidade, segurança e tecnologias.
  </li>
  <li>
    <strong>Exemplos:</strong>
    <ul>
      <li>
        <strong>Desempenho:</strong> O relatório deve ser gerado em até 5 segundos.
      </li>
      <li>
        <strong>Padrões:</strong> Todos os documentos devem seguir o layout do setor
        específico.
      </li>
      <li>
        <strong>Tecnologia:</strong> O sistema deve ser desenvolvido obrigatoriamente
        em linguagem Java.
      </li>
      <li>
        <strong>Disponibilidade:</strong> O sistema deve estar online 24 horas por
        dia.
      </li>
    </ul>
  </li>
</ul>

<h3>Trabalhando com Casos de Uso</h3>

<p>
  Os <strong>Casos de Uso</strong> são documentos utilizados em metodologias tradicionais
  para detalhar e modelar os requisitos funcionais de um software. Eles descrevem
  o comportamento do sistema por meio de sequências de passos, ações e comportamentos
  necessários para atingir um resultado satisfatório. Documentar um caso de uso significa
  listar o fluxo de eventos que evidencia o que cada funcionalidade deve executar.
</p>

<p>
  O detalhamento das funcionalidades em um caso de uso é organizado em três
  tipos de fluxos principais, que cobrem desde a execução perfeita até o
  tratamento de erros e funções opcionais. É fundamental adotar um padrão de
  documentação para que o entendimento seja uniforme entre todos os envolvidos,
  garantindo que o software seja construído corretamente.
</p>

<h4>Tipos de Fluxos de Eventos</h4>

<ul>
  <li>
    <strong>Fluxo Principal (FP):</strong> Também chamado de "caminho feliz", descreve
    o cenário onde todas as informações estão corretas e o objetivo principal é atingido
    sem interrupções ou erros. Exemplo: informar dados e salvar um cadastro com sucesso.
  </li>
  <li>
    <strong>Fluxo Alternativo (FA):</strong> Trata situações que fogem do caminho
    esperado, detalhando o passo a passo para lidar com informações incorretas ou
    ações não previstas. Exemplo: validar se um CPF é inválido ou se um nome contém
    caracteres proibidos.
  </li>
  <li>
    <strong>Fluxo de Exceção (FE):</strong> Contempla funções que não são obrigatórias
    para o objetivo principal, mas que estão disponíveis para o usuário durante o
    processo. Exemplo: opções de "alterar senha", "ajuda online" ou "consultar histórico".
  </li>
</ul>

<h4>Características Importantes</h4>

<ul>
  <li>
    <strong>Abrangência:</strong> Um único caso de uso pode descrever vários requisitos
    relacionados, como as ações de inserir, alterar, consultar e excluir um registro.
  </li>
  <li>
    <strong>Objetivo:</strong> Serve como guia para a implementação técnica, permitindo
    que a equipe opine sobre a melhor forma de construir a funcionalidade.
  </li>
  <li>
    <strong>Comunicação:</strong> Facilita a validação do comportamento do software
    antes da codificação.
  </li>
</ul>

<h3>Conclusão: Planejamento e Engenharia de Requisitos</h3>

<p>
  A construção de um software é uma tarefa complexa que exige um processo
  gradual e estruturado. O sucesso do projeto depende diretamente de quão bem os
  requisitos são compreendidos e documentados, garantindo que o sistema final
  funcione de maneira adequada para o usuário e atenda às suas reais
  necessidades.
</p>

<p>
  O ciclo de vida da engenharia de software destaca a importância da gestão
  contínua. Como as necessidades dos usuários e do mercado mudam constantemente,
  os requisitos devem evoluir de forma gerenciada. Isso assegura que qualquer
  alteração seja devidamente refletida e implementada, mantendo o software
  alinhado com os objetivos do negócio.
</p>

<h4>Recapitulação dos Conceitos Chave</h4>

<ul>
  <li>
    <strong>Gradualidade:</strong> O processo deve ser feito por etapas, priorizando
    o entendimento antes da definição técnica da construção.
  </li>
  <li>
    <strong>Gestão de Mudanças:</strong> Requisitos não são estáticos; é preciso
    gerenciar sua evolução para que o software não se torne obsoleto ou incorreto.
  </li>
  <li>
    <strong>Especificação de Requisitos:</strong> Documento que consolida a visão
    macro do que deve ser desenvolvido.
  </li>
  <li>
    <strong>Requisitos Funcionais e Não Funcionais:</strong> Divisão essencial entre
    o que o sistema faz (funcionalidades) e como ele se comporta (qualidade e restrições).
  </li>
</ul>
