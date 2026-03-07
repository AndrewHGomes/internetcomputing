<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Diagrama de Classes (UML)</h2>

<Audios modulo="M8" aulas={["17", "18", "19", "20"]} />

<p>
  O desenvolvimento de software não é uma tarefa trivial, exigindo a tradução de
  problemas reais em código. A base de todo o processo é a <strong>
    Engenharia de Requisitos
  </strong>, pois falhas na análise das necessidades do cliente comprometem a
  eficácia da solução final. O <strong>Diagrama de Classes</strong> surge como uma
  ferramenta essencial na etapa de projeto para modelar a estrutura do sistema.
</p>

<h4>Conceitos Fundamentais</h4>

<p>
  Segundo a UML, o Diagrama de Classes descreve as classes de um sistema e seus
  respectivos relacionamentos. Ele é fundamentado na <strong
    >Orientação a Objetos (OO)</strong
  >, que utiliza os seguintes pilares:
</p>

<ul>
  <li>
    <strong>Classe:</strong> Representa um conjunto de objetos com a mesma estrutura
    e comportamento.
  </li>
  <li>
    <strong>Objeto:</strong> Representação de um elemento do mundo real (ex: Cliente,
    Produto).
  </li>
  <li>
    <strong>Abstração:</strong> Foco apenas nos aspectos relevantes para o sistema,
    ignorando detalhes desnecessários.
  </li>
  <li>
    <strong>Encapsulamento:</strong> Esconde os detalhes internos de implementação,
    expondo apenas o que é necessário para a interação externa.
  </li>
  <li>
    <strong>Herança:</strong> Permite que classes compartilhem atributos e métodos
    através de uma hierarquia, facilitando o reaproveitamento de código.
  </li>
</ul>

<h4>Estrutura e Aplicação</h4>

<p>
  O diagrama modela como as informações se encaixam e se comunicam. Em um
  cenário escolar, por exemplo, as classes <strong
    >Aluno, Turma e Professor</strong
  > interagem entre si para refletir as regras de negócio da instituição. Essas conexões
  definem a dinâmica do software, garantindo que ele opere conforme a realidade do
  cliente.
</p>

<ul>
  <li>Modelagem da estrutura estática do sistema.</li>
  <li>
    Definição de como as classes se relacionam (ex: Aluno matriculado em Turma).
  </li>
  <li>Visualização da comunicação entre diferentes componentes do software.</li>
</ul>

<h3>Elementos do Diagrama de Classe</h3>

<p>
  A construção de um Diagrama de Classe exige uma organização lógica onde cada
  elemento deve estar em seu devido lugar. O princípio fundamental é que as
  responsabilidades sejam atribuídas corretamente: as ações de um aluno devem
  pertencer à classe <strong>Aluno</strong>, e não à classe Professor, por
  exemplo. Isso garante que a estrutura do software reflita fielmente as regras
  de negócio.
</p>

<h4>Componentes Principais</h4>

<p>
  Para modelar o sistema, utilizamos quatro elementos fundamentais que definem a
  estrutura e o comportamento dos objetos:
</p>

<ul>
  <li>
    <strong>Classes:</strong> Representam os objetos do mundo real pertinentes ao
    escopo do software (ex: Aluno, Turma, Professor).
  </li>
  <li>
    <strong>Atributos:</strong> São as características, propriedades ou estados de
    uma classe. Definem o que a classe "sabe" sobre si mesma (ex: nome, matrícula,
    preço).
  </li>
  <li>
    <strong>Métodos (Operações):</strong> Representam as ações ou funções sob responsabilidade
    da classe. Definem o que a classe "faz" (ex: Matricular Aluno, Calcular Média).
  </li>
  <li>
    <strong>Relacionamentos:</strong> Demonstram como as classes interagem e trocam
    informações entre si para executar as funcionalidades do sistema.
  </li>
</ul>

<h4>Processo de Modelagem</h4>

<p>O raciocínio para criar o diagrama segue uma sequência lógica:</p>

<ol>
  <li>
    Identificar as <strong>Classes</strong> dentro do contexto do software.
  </li>
  <li>
    Definir os <strong>Atributos</strong> necessários para caracterizar cada classe.
  </li>
  <li>Determinar os <strong>Métodos</strong> que cada classe deve executar.</li>
  <li>
    Estabelecer os <strong>Relacionamentos</strong> para mostrar como esses objetos
    colaboram para processar os requisitos.
  </li>
</ol>

<h3>Estrutura da Classe: Atributos e Métodos</h3>

<p>
  Uma classe é a abstração de um conjunto de elementos que compartilham
  características e comportamentos. Na UML, a classe é representada visualmente
  por um retângulo dividido em seções que organizam sua identidade, dados e
  ações.
</p>

<h4>Padronização de Nomenclatura</h4>

<p>
  Para garantir a organização e a manutenção do sistema, as classes devem seguir
  o <strong>vocabulário do dicionário de dados</strong>. Isso significa que o
  nome dado a uma classe (ex: CLIENTE) deve ser o mesmo utilizado nos
  requisitos, na documentação e nas variáveis do código-fonte, mantendo a
  consistência em todo o projeto.
</p>

<h4>Atributos (Características)</h4>

<p>
  Os atributos definem as propriedades e estados de um objeto. Cada atributo
  possui um <strong>tipo de dado</strong> específico, que delimita o intervalo de
  valores permitidos para aquela propriedade.
</p>

<ul>
  <li>
    <strong>Exemplos de Tipos:</strong> O nome de um aluno é do tipo "texto" (string),
    enquanto o número de sua matrícula é do tipo "inteiro".
  </li>
  <li>
    <strong>Instância:</strong> Quando preenchemos os atributos de uma classe com
    dados reais (ex: Nome: "João", CPF: "123..."), criamos uma instância ou objeto
    específico daquela classe.
  </li>
</ul>

<h4>Métodos (Operações)</h4>

<p>
  Os métodos são as funções ou serviços que a classe disponibiliza ao sistema.
  Eles representam as responsabilidades de execução de cada objeto. No caso de
  uma classe ALUNO, os métodos seriam as operações lógicas necessárias para
  manipulá-la, como Consultar Aluno ou Alterar Dados.
</p>

<h3>Relacionamentos entre Classes</h3>

<p>
  O objetivo dos relacionamentos é garantir a comunicação e a colaboração entre
  as classes. Eles definem como as informações são compartilhadas e como as
  regras de negócio são aplicadas no sistema.
</p>

<h4>Características de um Relacionamento</h4>

<p>
  Para compreender como as classes interagem, analisa-se os seguintes elementos:
</p>

<ul>
  <li>
    <strong>Nome e Sentido:</strong> Descrição da ação (ex: "trabalha para") e a
    direção da leitura (origem para destino).
  </li>
  <li>
    <strong>Navegabilidade:</strong> Indicada por uma seta, mostra qual classe "enxerga"
    a outra.
  </li>
  <li>
    <strong>Multiplicidade:</strong> Define a quantidade de objetos envolvidos no
    relacionamento (ex: 1..1, 0..*, 1..3). É crucial para validar as regras do software.
  </li>
  <li>
    <strong>Papéis:</strong> A função que cada classe desempenha naquela relação
    específica (ex: Empregado e Empregador).
  </li>
</ul>

<h4>Tipos de Relacionamentos (UML)</h4>

<p>
  A UML define três tipos principais de conexões, cada uma com um propósito e
  representação visual distintos:
</p>

<ol>
  <li>
    <strong>Associação:</strong> Indica um vínculo simples entre objetos de
    classes diferentes. É representada por uma linha sólida.
    <ul>
      <li>
        <strong>Exemplo:</strong> Uma Pessoa trabalha para uma Empresa. Elas estão
        vinculadas, mas mantêm suas existências independentes.
      </li>
    </ul>
  </li>
  <li>
    <strong>Generalização (Herança):</strong> Relaciona uma "classe mãe"
    (superclasse) a "classes filhas" (subclasses). As filhas herdam todos os
    atributos e métodos da mãe, mas podem ter características próprias.
    <ul>
      <li>
        <strong>Exemplo:</strong> Veículo é a superclasse. Terrestre e Aéreo são
        subclasses que herdam as propriedades gerais de um veículo.
      </li>
    </ul>
  </li>
  <li>
    <strong>Dependência: </strong>Indica que uma classe utiliza outra ou é
    afetada por mudanças nela. É representada por uma linha tracejada com seta.
    <ul>
      <li>
        <strong>Exemplo:</strong> Se a classe Funcionário for removida, a classe
        Dependentes perde sua razão de existir no contexto do sistema.
      </li>
    </ul>
  </li>
</ol>

<h3>Passo a Passo para Modelagem</h3>

<p>
  A modelagem de um Diagrama de Classe não é intuitiva; ela é o resultado final
  de um processo de análise que transforma necessidades subjetivas do cliente em
  especificações objetivas. O sucesso do diagrama depende diretamente da
  qualidade do levantamento de requisitos realizado previamente.
</p>

<h4>O Fluxo de Trabalho (Pipeline)</h4>

<p>
  Para construir um diagrama eficiente, deve-se seguir esta sequência lógica:
</p>

<ol>
  <li>
    <strong>Entendimento do Negócio:</strong> Modelar o fluxo de processos de negócio.
  </li>
  <li>
    <strong>Especificação de Requisitos:</strong> Listar o que o software deve fazer.
  </li>
  <li>
    <strong>Diagrama de Casos de Uso:</strong> Identificar atores e funcionalidades.
  </li>
  <li>
    <strong>Detalhamento (Descrição) dos Casos de Uso:</strong> Compreender o funcionamento
    interno de cada requisito funcional para identificar quais objetos participam
    da ação.
  </li>
  <li>
    <strong>Identificação de Classes:</strong> Isolar as classes essenciais que representam
    o mundo real dentro do escopo do software.
  </li>
</ol>

<h4>Construção do Diagrama</h4>

<p>
  Após identificar as classes, o foco passa para o detalhamento técnico e
  estrutural:
</p>

<ul>
  <li>
    <strong>Definição de Atributos e Métodos:</strong> Listar quais informações cada
    classe armazena e quais ações ela executa.
  </li>
  <li>
    <strong>Estabelecimento de Relacionamentos:</strong> Conectar as classes definindo
    nome, navegabilidade e multiplicidade.
  </li>
  <li>
    <strong>Refinamento das Regras de Negócio:</strong> Ajustar os relacionamentos
    para que reflitam exatamente como os dados devem ser processados (ex: garantir
    que um aluno só possa estar em uma turma por vez, se essa for a regra).
  </li>
</ul>

<h4>Considerações Finais</h4>

<p>
  Não existe uma "resposta única" na modelagem. Diferentes analistas podem
  identificar conjuntos de classes distintos para o mesmo problema, dependendo
  da lógica de implementação escolhida. O objetivo final é sempre garantir que o
  diagrama seja uma planta fiel para a codificação, resolvendo o problema do
  cliente de forma eficiente.
</p>

<h3>Conclusão: A Transição do Lógico para o Físico</h3>

<p>
  Esta etapa finaliza a compreensão do <strong>Diagrama de Classes</strong> como
  a ponte entre a necessidade do cliente e a construção real do sistema.
  Enquanto o Diagrama de Casos de Uso foca no que o software deve fazer (visão
  lógica), o Diagrama de Classes foca em
  <strong>como ele será implementado</strong> (visão física/estrutural).
</p>

<h4>Pontos Chave da Modelagem de Sistemas</h4>

<ul>
  <li>
    Trabalho Contínuo: A modelagem não é estática. Cada etapa (Requisitos &gt;
    Casos de Uso &gt; Diagrama de Classes) alimenta a seguinte com informações
    essenciais.
  </li>
  <li>
    Visão Estrutural: O Diagrama de Classes organiza o software como algo
    concreto, definindo a arquitetura que os desenvolvedores irão codificar.
  </li>
  <li>
    Valor ao Cliente: Um sistema bem modelado resulta em um software mais
    robusto, fácil de manter e que realmente resolve os problemas identificados
    na fase de requisitos.
  </li>
</ul>

<h4>Fluxo de Aprendizado</h4>

<ul>
  <li>
    Casos de Uso:
    <ul>
      <li>
        Lógico Funcional:
        <ul>
          <li>Endender as intenções do usuário e funções do sistema.</li>
        </ul>
      </li>
    </ul>
  </li>
  <li>
    Diagrama de Classes:
    <ul>
      <li>
        Físico/Estrutural:
        <ul>
          <li>Projetar a arquitetura, dados e comportamentos do código.</li>
        </ul>
      </li>
    </ul>
  </li>
</ul>
