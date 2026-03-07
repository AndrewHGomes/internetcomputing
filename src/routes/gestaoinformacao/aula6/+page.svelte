<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Inteligência do Negócio</h2>

<Audios modulo="M2" aulas={["21", "22", "23", "24"]} />

<p>
  A <strong>gestão da informação</strong> é um processo dinâmico e contínuo,
  onde novas necessidades surgem constantemente. Para manter a
  <strong>competitividade</strong>, as organizações precisam fornecer
  informações completas e precisas com agilidade. Isso exige uma
  <strong>gestão do conhecimento</strong>
  eficiente e mecanismos de <strong>segurança da informação</strong> que
  garantam a <strong>confidencialidade</strong>,
  <strong>disponibilidade</strong>
  e <strong>integridade</strong> dos dados.
</p>

<p>
  O <strong>Business Intelligence (BI)</strong>, ou Inteligência de Negócios,
  surge como uma resposta à necessidade de extrair valor dos dados. Ele é um
  conjunto de práticas, metodologias e tecnologias que transforma grandes
  volumes de <strong>dados desorganizados</strong> em informações estratégicas.
  Seu foco principal é oferecer <strong>suporte à tomada de decisão</strong> e monitorar
  os resultados de investimentos em todos os setores da empresa.
</p>

<p>
  O funcionamento do BI depende da integração entre <strong>negócio</strong>,
  <strong>gestão</strong>
  e <strong>TI</strong>. Ele possui a flexibilidade de captar dados de diversas
  fontes, como sistemas internos e bancos de dados pré-existentes, permitindo a
  identificação de <strong>oportunidades</strong> e a mitigação de
  <strong>riscos</strong>.
</p>

<p>
  Em resumo, o BI é um <strong>processo orientado por tecnologia</strong> que
  utiliza ferramentas e aplicativos para coletar, analisar e apresentar
  informações úteis. Essas ferramentas podem incluir o uso de
  <strong>inteligência artificial</strong> para realizar consultas complexas e análises
  preditivas que atendam às necessidades específicas da alta gestão.
</p>

<ul>
  <li>
    Transformação de dados brutos em <strong>conhecimento estratégico</strong>.
  </li>
  <li>Suporte direto à <strong>tomada de decisão</strong>.</li>
  <li>
    Integração de dados de <strong>fontes heterogêneas</strong> (internas e externas).
  </li>
  <li>
    Melhoria da <strong>agilidade organizacional</strong> e competitividade.
  </li>
  <li>
    Monitoramento contínuo de <strong>indicadores de desempenho</strong>.
  </li>
</ul>

<h3>Big Data</h3>

<p>
  O termo <strong>Big Data</strong> refere-se a conjuntos de dados extremamente
  amplos e complexos que exigem tecnologias específicas para processamento e
  armazenamento, superando a capacidade dos softwares tradicionais. O objetivo
  central é transformar esse grande volume de informações em soluções para
  problemas de negócios que antes eram insolúveis. A base conceitual do Big Data
  evoluiu dos chamados <strong>3Vs</strong> para os <strong>5Vs</strong>, que
  definem suas características principais:
</p>

<ol>
  <li>
    <strong>Volume</strong>: Trata da imensa quantidade de dados gerados,
    incluindo dados não estruturados provenientes de redes sociais, sensores e
    aplicativos móveis.
  </li>
  <li>
    <strong>Velocidade</strong>: Refere-se à rapidez com que os dados são
    recebidos e processados, muitas vezes em tempo real, exigindo estratégias
    como o processamento em memória.
  </li>
  <li>
    <strong>Variedade</strong>: Abrange a diversidade de formatos, desde dados
    estruturados (bancos de dados relacionais) até não estruturados e
    semiestruturados, como textos, áudios e vídeos.
  </li>
  <li>
    <strong>Veracidade</strong>: Diz respeito à confiabilidade e qualidade dos
    dados, filtrando inconsistências e informações falsas para garantir que as
    decisões sejam baseadas em fontes seguras.
  </li>
  <li>
    <strong>Valor</strong>: Relaciona-se à utilidade prática dos dados para o
    negócio, garantindo que o processamento resulte em benefícios reais e
    decisões estratégicas para a empresa.
  </li>
</ol>

<p>
  O tratamento desses dados exige um pré-processamento para lidar com a
  complexidade de <strong>metadados</strong> e garantir que as informações sejam
  coerentes com as necessidades do mercado. Atualmente, a demanda por profissionais
  capacitados em Big Data é alta devido à sua importância estratégica na geração
  de inteligência competitiva.
</p>

<h3>Data Warehouse</h3>

<p>
  O <strong>Data Warehouse</strong> é traduzido como um
  <strong>armazém de dados</strong>, funcionando como um repositório digital que
  organiza e centraliza informações provenientes de diversas fontes, tanto
  internas quanto externas. Sua principal função é servir de base para o
  <strong>processamento e armazenamento de altos volumes de dados</strong>,
  permitindo que a empresa realize análises complexas e gere relatórios
  essenciais para a <strong>tomada de decisão estratégica</strong>.
</p>

<p>
  Surgido na década de 1980, o conceito possui forte ligação com o <strong
    >Big Data</strong
  >
  e o
  <strong>Business Intelligence</strong> (BI). Embora sejam frequentemente
  confundidos, o DW e o BI são distintos: o Data Warehouse é o
  <strong>sistema de armazenamento</strong>
  técnico, enquanto o BI é a <strong>gestão estratégica</strong> que utiliza esses
  dados. Em suma, o DW alimenta o BI, garantindo que grandes volumes de dados estejam
  disponíveis e estruturados para uso executivo.
</p>

<p>
  Para explorar as informações contidas em um armazém de dados, utiliza-se a
  ferramenta <strong>OLAP (Online Analytical Processing)</strong>. Essa
  tecnologia permite analisar grandes quantidades de dados sob
  <strong>múltiplas perspectivas</strong> e em tempo real. Sua aplicação é
  versátil, abrangendo desde a área <strong>financeira</strong> (fluxo de caixa
  e orçamentos) e <strong>marketing</strong> (análise de preços e mercado) até o
  setor de <strong>vendas</strong> (previsões de faturamento e lucro). A implementação
  de um DW oferece vantagens e desvantagens que devem ser pesadas:
</p>

<ul>
  <li>
    <strong>Vantagens:</strong> Identificação de
    <strong>inconsistências</strong>
    antes do carregamento dos dados, maior precisão em
    <strong>relatórios de tendências</strong> e comparação eficiente entre objetivos
    previstos e desempenho real.
  </li>
  <li>
    <strong>Desvantagens:</strong> Inadequação para lidar com
    <strong>dados não estruturados, custos elevados</strong> de implementação e o
    risco de obsolescência tecnológica rápida.
  </li>
</ul>

<p>
  Em resumo, o Data Warehouse consolida <strong>informações históricas</strong>
  em um banco de dados robusto. Ele transforma o volume bruto de dados em conhecimento
  organizado, permitindo que as organizações obtenham
  <strong>previsões</strong> seguras e uma visão clara do seu posicionamento e futuro.
</p>

<h3>Data Mining</h3>

<p>
  O <strong>Data Mining</strong>, ou <strong>mineração de dados</strong>,
  refere-se a sistemas computacionais projetados para vasculhar grandes
  repositórios de informações em busca de <strong>conhecimento oculto</strong>.
  Seu principal desafio é separar o que é dado relevante para o negócio daquilo
  que é apenas
  <strong>ruído</strong> (informação irrelevante). Essa tecnologia é amplamente percebida
  em estratégias de marketing digital, onde o comportamento do usuário é processado
  para oferecer produtos específicos de seu interesse.
</p>

<p>
  O propósito central da ferramenta é identificar <strong>padrões</strong>,
  consistências e relacionamentos entre dados que, à primeira vista, parecem
  desconexos. Ao descobrir essas ligações, as empresas conseguem transformar
  dados brutos em
  <strong>conhecimento estratégico</strong>, permitindo otimizar resultados
  financeiros e realizar <strong>projeções futuras</strong> com base em comportamentos
  de consumo e perfis de clientes.
</p>

<p>
  Para ser efetivo, o processo de mineração deve percorrer etapas estruturadas
  em todas as áreas da organização:
</p>

<ul>
  <li>
    <strong>Identificação do problema:</strong> Definição clara do objetivo ou meta
    a ser alcançada.
  </li>
  <li>
    <strong>Descoberta do conhecimento:</strong> Uso de
    <strong>inteligência artificial</strong> para identificar relações complexas
    entre os dados.
  </li>
  <li>
    <strong>Análise das relações descobertas:</strong> Avaliação (manual ou automatizada)
    da relevância das conexões encontradas.
  </li>
  <li>
    <strong>Uso das relações descobertas:</strong> Aplicação prática das
    informações na <strong>gestão do negócio</strong> e tomada de decisões.
  </li>
  <li>
    <strong>Avaliação dos resultados:</strong> Verificação da utilidade das descobertas
    e se os objetivos iniciais foram atingidos.
  </li>
</ul>

<h3>Tomada de Decisão</h3>

<p>
  A <strong>tomada de decisão</strong> eficaz é o diferencial competitivo que
  permite às empresas se destacarem e agirem com rapidez. No cenário
  corporativo, decidir envolve analisar diferentes alternativas e escolher a
  mais adequada para a situação, o que exige o descarte de outras opções. Quando
  esse processo é fundamentado em
  <strong>dados reais, corretos e relevantes</strong>, os resultados tendem a
  ser mais assertivos e os riscos são minimizados.
</p>

<p>
  A necessidade crescente de gerenciar informações deve-se à <strong>
    velocidade alucinante
  </strong>
  do mundo atual e ao volume massivo de dados gerados constantemente pelas pessoas.
  A tecnologia permite que as empresas monitorem comportamentos, hábitos de consumo
  e preferências em tempo real. O grande desafio, portanto, não é a falta de dados,
  mas sim a capacidade de criar
  <strong>filtros de informações relevantes</strong> para encontrar os relacionamentos
  que realmente apoiam a estratégia do negócio.
</p>

<p>
  As técnicas de coleta e organização, como as estudadas anteriormente, são
  <strong>complementares</strong> e essenciais para a sustentabilidade
  organizacional. Elas transformam o excesso de dados em
  <strong>informação coerente</strong>, agregando valor ao negócio e garantindo
  que os gestores tenham uma base sólida para guiar o futuro da empresa em um
  mercado altamente competitivo.
</p>

<h3>Conclusão: Transformação Digital e Inteligência Artificial</h3>

<p>
  A <strong>transformação digital</strong> nas empresas prioriza a
  <strong>velocidade</strong>
  e a
  <strong>qualidade</strong> da informação. A estabilidade e o futuro das
  organizações dependem diretamente da capacidade de converter grandes volumes
  de dados em conhecimento estratégico. Por isso, o investimento em tecnologias
  para armazenar, processar e utilizar dados é o que garante decisões mais
  <strong>precisas e assertivas</strong>, aumentando a competitividade no
  mercado.
</p>

<p>
  As técnicas de <strong>Data Warehouse</strong> e <strong>Data Mining</strong>
  integram o campo da <strong>Inteligência Artificial (IA)</strong>, que se
  consolidou como um diferencial competitivo essencial para lidar com a
  complexidade dos negócios modernos. A IA atua como uma aliada na navegação de
  grandes massas de dados, permitindo que a empresa identifique oportunidades e
  riscos com maior clareza.
</p>
