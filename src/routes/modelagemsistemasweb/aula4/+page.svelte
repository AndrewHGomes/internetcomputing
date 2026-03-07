<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Revisão de Etapas Anteriores</h2>

<Audios modulo="M8" aulas={["13", "14", "15", "16"]} />

<p>
  O ciclo de desenvolvimento inicia com o entendimento e modelagem dos <strong>
    processos de negócio
  </strong>, visando identificar falhas e melhorias (processo TO BE). Em
  seguida, foca-se nos <strong>dados</strong>, sua entrada, armazenamento e
  relacionamentos, pois são a base para o processamento do software. Por fim,
  definem-se os <strong>requisitos</strong>
  (funcionais e não funcionais), que são documentados e detalhados em
  <strong>casos de uso</strong>
  para garantir que a funcionalidade desejada seja clara e completa.
</p>

<h3>O que é UML (Unified Modelling Language)?</h3>

<p>
  A UML é uma linguagem de modelagem padrão utilizada para especificar,
  visualizar e documentar projetos de software orientados a objetos. Ela
  funciona como uma <strong>notação gráfica</strong> universal, facilitando a
  comunicação entre os envolvidos no projeto. É importante ressaltar que a UML
  <strong>não é um método ou processo</strong> de desenvolvimento (não dita a ordem
  das tarefas), mas sim uma ferramenta de comunicação visual padronizada pela OMG
  (Object Management Group).
</p>

<h4>Contexto Histórico e o RUP</h4>

<p>
  A UML surgiu na década de 90 (Booch e Rumbaugh) na Rational Software,
  impulsionada pela necessidade de formalizar o desenvolvimento de sistemas
  complexos. Nesse contexto, nasceu o <strong
    >RUP (Rational Unified Process)</strong
  >, um processo de desenvolvimento unificado que se tornou referência em
  metodologias tradicionais de software, utilizando a UML como sua base de
  modelagem visual.
</p>

<h4>Modelagem e Visões da UML</h4>

<p>
  Na engenharia de software, um <strong>modelo</strong> é uma abstração ou simplificação
  da realidade, construído para facilitar a compreensão do sistema antes da codificação.
  Segundo a UML, o software deve ser compreendido sob duas perspectivas complementares:
</p>

<ul>
  <li>
    <strong>Visão Estrutural:</strong> Foca na organização do sistema, identificando
    seus componentes e como eles estão estaticamente relacionados.
  </li>
  <li>
    <strong>Visão Comportamental:</strong> Foca na dinâmica do sistema, descrevendo
    como os elementos interagem, se comunicam e respondem a estímulos ao longo do
    tempo.
  </li>
</ul>

<h3>Modelos e Diagramas da UML</h3>

<p>
  Os diagramas são representações visuais da solução de software baseadas nos
  requisitos. Eles são divididos conforme o que pretendem comunicar:
</p>

<h4>Diagramas Estruturais (Estáticos)</h4>

<ul>
  <li>
    <strong>Diagrama de Classes:</strong> O mais importante da orientação a objetos.
    Descreve as classes, seus atributos (dados), métodos (ações) e como elas se relacionam.
  </li>
  <li>
    <strong>Diagrama de Componentes:</strong> Foca na organização física do código,
    como bibliotecas, módulos, arquivos executáveis e códigos-fonte.
  </li>
  <li>
    <strong>Diagrama de Implantação:</strong> Modela a infraestrutura de hardware
    onde o software será instalado (servidores de desenvolvimento, teste e produção).
  </li>
</ul>

<h4>Diagramas Comportamentais (Dinâmicos)</h4>

<ul>
  <li>
    <strong>Diagrama de Casos de Uso:</strong> Especifica os requisitos funcionais,
    mostrando como os atores (usuários ou sistemas) interagem com o software.
  </li>
  <li>
    <strong>Diagrama de Sequência:</strong> Mostra a interação entre objetos ao longo
    do tempo, detalhando a ordem das mensagens trocadas.
  </li>
  <li>
    <strong>Diagrama de Atividades:</strong> Modela o fluxo de processos ou a lógica
    de um algoritmo. É a versão UML para fluxogramas de negócio.
  </li>
  <li>
    <strong>Diagrama de Estados:</strong> Descreve as mudanças de estado de um objeto
    específico conforme ele recebe estímulos externos durante seu ciclo de vida.
  </li>
</ul>

<h4>Aplicação Prática e Agilidade</h4>

<p>Embora a UML ofereça diversos diagramas, o uso deve ser estratégico:</p>

<ul>
  <li>
    <strong>Valor Agregado:</strong> Deve-se utilizar apenas os diagramas que facilitem
    a compreensão da equipe e melhorem a qualidade.
  </li>
  <li>
    <strong>Evitar Desperdício:</strong> Não é necessário criar todos os diagramas
    para todos os projetos; a escolha depende da complexidade e da necessidade de
    documentação.
  </li>
  <li>
    <strong>Base:</strong> A UML é construída sob as premissas da
    <strong>Orientação a Objetos</strong>.
  </li>
</ul>

<h3>O Conceito de Objeto</h3>

<p>
  Na orientação a objetos, os elementos da solução são representados como
  <strong>objetos</strong>. Um objeto é a base do modelo e representa algo
  identificável do mundo real, podendo ser:
</p>

<ul>
  <li><strong>Físico:</strong> Um carro, uma pessoa.</li>
  <li><strong>Conceitual:</strong> Um diagrama, um processo.</li>
  <li><strong>De Software:</strong> Um botão (checkbox), uma janela.</li>
</ul>

<h4>Pilares do Objeto</h4>

<ul>
  <li>
    <strong>Identidade:</strong> O que torna o objeto único e permite que seja referenciado.
  </li>
  <li>
    <strong>Atributos (Características):</strong> Propriedades mutáveis que descrevem
    o objeto.
  </li>
  <li>
    <strong>Métodos (Comportamento):</strong> Como o objeto reage a estímulos e interage
    com outros.
  </li>
</ul>

<h3>Conceitos Fundamentais da OO</h3>

<h4>Abstração</h4>

<p>
  Consiste em focar apenas nos aspectos <strong>essenciais</strong> e relevantes
  de um objeto para um determinado propósito, ignorando detalhes acidentais ou desnecessários.
  Serve para simplificar a complexidade.
</p>

<h4>Encapsulamento</h4>

<p>
  É a técnica de esconder os detalhes internos da implementação de um objeto.
</p>

<ul>
  <li>
    <strong>Interface:</strong> O objeto mostra apenas "o que faz" (externo).
  </li>
  <li><strong>Privacidade:</strong> O "como faz" (interno) fica oculto.</li>
  <li>
    <strong>Exemplo:</strong> Você usa o acelerador de um carro (interface) sem precisar
    entender a mecânica da injeção de combustível (detalhe interno).
  </li>
</ul>

<h4>Herança</h4>

<p>
  Permite o compartilhamento de atributos e comportamentos entre objetos através
  de uma hierarquia.
</p>

<ul>
  <li>
    Objetos em níveis inferiores herdam características dos níveis superiores.
  </li>
  <li>
    <strong>Objetivo:</strong> Evitar redundância e reaproveitar estruturas comuns.
  </li>
</ul>

<p>
  A <strong>Orientação a Objetos</strong> facilita a análise de problemas complexos
  ao organizar o sistema em coleções de objetos e métodos, tornando o software mais
  flexível e fácil de manter.
</p>

<h3>O que é o Diagrama de Casos de Uso?</h3>

<p>
  É geralmente o primeiro diagrama construído após o levantamento de requisitos.
  Seu objetivo é mostrar o <strong>comportamento externo</strong> do software, focando
  no que o sistema faz e não em como ele será implementado. Serve como uma ferramenta
  de comunicação para validar o escopo com o cliente.
</p>

<h4>Elementos do Diagrama</h4>

<p>
  O diagrama utiliza uma notação simples para representar a interação entre o
  usuário e o sistema:
</p>

<ul>
  <li>
    <strong>Atores (Bonecos):</strong> Representam os usuários ou sistemas externos
    que interagem com o software.
  </li>
  <li>
    <strong>Casos de Uso (Elipses):</strong> Representam as funcionalidades ou serviços
    oferecidos pelo sistema.
  </li>
  <li>
    <strong>Relacionamentos (Linhas):</strong> Indicam a conexão e a interação entre
    atores e casos de uso.
  </li>
  <li>
    <strong>Limites do Sistema (Retângulo):</strong> Representa a fronteira do software.
    Os casos de uso (escopo) ficam dentro, enquanto os atores ficam fora.
  </li>
</ul>

<h4>Finalidade e Aplicação</h4>

<p>
  O diagrama permite visualizar o relacionamento entre as funcionalidades e os
  responsáveis por executá-las.
</p>

<ul>
  <li>
    <strong>Validação de Requisitos:</strong> Ajuda a conferir se o entendimento
    do sistema está correto e completo.
  </li>
  <li>
    <strong>Visão de Processo:</strong> Modela visualmente o fluxo do negócio para
    garantir que todas as necessidades sejam atendidas.
  </li>
  <li>
    <strong>Exemplo Prático:</strong> Em uma máquina de self-service, os atores seriam
    o "Cliente", o "Reabastecedor" e o "Coletor". Cada um interage com casos de uso
    específicos (comprar produto, repor estoque, retirar dinheiro).
  </li>
</ul>

<h3>Elementos do Diagrama de Caso de Uso</h3>

<h4>Ator</h4>

<p>
  Representa o papel de uma entidade externa (pessoa ou outro sistema) que troca
  informações com o software.
</p>

<ul>
  <li>
    <strong>Características:</strong> Interage com o sistema, mas está fora de sua
    fronteira.
  </li>
  <li>
    <strong>Flexibilidade:</strong> Um usuário real pode atuar como vários atores,
    e um ator pode ser representado por múltiplos usuários.
  </li>
  <li>
    <strong>Representação:</strong> Desenho de um "boneco" com o nome do papel abaixo.
  </li>
</ul>

<h4>Caso de Uso</h4>

<p>Define uma funcionalidade ou serviço específico do sistema.</p>

<ul>
  <li>
    <strong>Foco:</strong> Deve-se modelar primeiro o fluxo principal e, depois,
    os fluxos alternativos e de exceção.
  </li>
  <li>
    <strong>Representação:</strong> Uma elipse com o nome da função em seu interior.
  </li>
</ul>

<h3>Relacionamentos entre Casos de Uso</h3>

<p>
  Os relacionamentos definem a dinâmica entre as funcionalidades e são
  essenciais para entender a lógica do negócio.
</p>

<h4>Inclusão (&lt;&lt;include&gt;&gt;)</h4>

<p>
  Indica uma funcionalidade <strong>obrigatória</strong> e essencial para o caso
  de uso principal.
</p>

<ul>
  <li>
    <strong>Conceito:</strong> O caso de uso B "faz parte de" A. Sem B, o caso de
    uso A não se completa.
  </li>
  <li>
    <strong>Exemplo:</strong> Para <strong>Efetuar Saque</strong>, é obrigatório
    <strong>Autenticar Cliente</strong>.
  </li>
</ul>

<h4>Extensão (&lt;&lt;extend&gt;&gt;)</h4>

<p>
  Indica uma funcionalidade opcional ou condicional que pode ser adicionada ao
  caso de uso principal.
</p>

<ul>
  <li>
    <strong>Conceito:</strong> O caso de uso B só ocorre em situações específicas
    ou por escolha do usuário.
  </li>
  <li>
    <strong>Exemplo:</strong> Ao finalizar uma operação, o sistema pode oferecer
    <strong>Contratar Seguro</strong> (o usuário decide se aceita ou não).
  </li>
</ul>

<h3>Síntese do Modelo</h3>

<p>A construção correta exige:</p>

<ol>
  <li>Identificação clara de todos os <strong>Atores</strong>.</li>
  <li>
    Mapeamento de todos os <strong>Casos de Uso</strong> (funcionalidades).
  </li>
  <li>
    Definição dos <strong>Relacionamentos</strong> e das
    <strong>Fronteiras</strong> do software (o que está dentro e o que está fora
    do sistema).
  </li>
</ol>

<h3>Conclusão</h3>

<p>
  A UML fornece uma visão visual e completa da solução de software através de
  seus diversos diagramas. O <strong>Diagrama de Caso de Uso</strong>, foco
  desta etapa, é a ferramenta essencial para definir o <strong>escopo</strong>,
  mapeando quem são os atores e como as funcionalidades se relacionam.
</p>

<h4>Pontos-Chave</h4>

<ul>
  <li>
    <strong>Objetivo:</strong> Mostrar o relacionamento entre atores e funções do
    sistema.
  </li>
  <li>
    <strong>Foco:</strong> Entender a dinâmica e o comportamento externo do software.
  </li>
  <li>
    <strong>Utilidade:</strong> Facilitar a comunicação e garantir que todas as necessidades
    do projeto sejam visualizadas antes da construção.
  </li>
</ul>
