<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Introdução aos Sistemas Embarcados</h2>

<Audios modulo="M3" aulas={["21", "22", "23", "24"]} />

<p>
  É comum sentir que o entendimento está apenas começando nesta etapa final dos
  estudos. O objetivo agora é conhecer os sistemas embarcados, seus componentes
  e aplicações, além de diferenciar microprocessadores e microcontroladores.
  Nesta etapa, o conteúdo abordará:
</p>

<ul>
  <li>Sistemas embarcados (definições).</li>
  <li>Diferenças entre microcontroladores e microprocessadores.</li>
  <li>Exemplos de microcontroladores e microprocessadores.</li>
  <li>Exemplos de programas em assembly e C para microcontroladores.</li>
  <li>Aplicações dos sistemas embarcados.</li>
</ul>

<h3>O que são Sistemas Embarcados</h3>

<p>
  Dispositivos como calculadoras, celulares, televisões, fornos de micro-ondas e
  máquinas de lavar possuem computadores acoplados, sem a necessidade de
  periféricos como monitor, teclado ou mouse. A capacidade de processamento
  desses computadores depende diretamente da aplicação de cada aparelho.
  Sistemas embarcados são pequenos sistemas microprocessados, programados e
  implementados em lugares específicos para fins específicos. O computador, ou
  controlador, fica incorporado (embarcado) ao próprio sistema que ele controla.
  Esses sistemas são caracterizados por possuírem:
</p>

<ul>
  <li>Baixo consumo de energia.</li>
  <li>Custo reduzido.</li>
  <li>Tempo de resposta rápido.</li>
  <li>
    Recursos de hardware e software otimizados em custo, dimensões e
    processamento.
  </li>
</ul>

<h3>Microprocessadores</h3>

<p>
  Os microprocessadores (ou processadores) são circuitos integrados formados por
  milhões de transistores. Eles realizam as funções de cálculo e tomada de
  decisão de um computador. Suas ações são coordenadas pelo <strong
    >clock</strong
  >, um sinal pulsante de frequência fixa gerado, na maioria dos casos, por um
  cristal de quartzo. O clock funciona como um maestro, sincronizando as ações
  do processador com as subidas e descidas de seu pulso. O funcionamento do
  microprocessador ocorre de forma cíclica e sincronizada em três passos:
</p>

<ol>
  <li>
    <strong>Entrada de dados digitais:</strong> o processador recebe informações
    externas.
  </li>
  <li>
    <strong>Processamento:</strong> os dados são processados de acordo com a memória
    e o programa.
  </li>
  <li>
    <strong>Saída de dados digitais:</strong> o processador envia as respostas para
    os elementos externos.
  </li>
</ol>

<h3>Componentes e Periféricos</h3>

<p>
  Periféricos são os componentes agregados ao processador para realizar o
  armazenamento ou a troca de dados com o mundo externo.
</p>

<h4>Memórias</h4>

<p>Responsáveis por armazenar dados, dividem-se em duas classificações:</p>

<ul>
  <li>
    <strong>Voláteis:</strong> Necessitam de alimentação contínua para manter as
    informações, mas possuem manipulação rápida. Exemplo: Memória RAM (guarda as
    variáveis durante a execução dos programas).
  </li>
  <li>
    <strong>Não voláteis:</strong> São mais lentas, porém retêm os dados sem
    energia. Exemplos:
    <ul>
      <li>
        <strong>ROM:</strong> Gravada na fabricação (ex: cartuchos de videogame).
      </li>
      <li>
        <strong>PROM:</strong> Gravada uma única vez com dispositivos especiais.
      </li>
      <li>
        <strong>EPROM:</strong> Pode ser apagada por exposição a luz ultravioleta
        (UV).
      </li>
      <li>
        <strong>EEPROM:</strong> Pode ser escrita e apagada eletricamente no próprio
        circuito.
      </li>
      <li>
        <strong>Flash:</strong> Tecnologia baseada na EEPROM, porém mais rápida (ex:
        pendrives, cartões SD e celulares).
      </li>
    </ul>
  </li>
</ul>

<h4>Conversores DA e AD</h4>

<p>Servem para traduzir informações digitais em analógicas e vice-versa.</p>

<ul>
  <li>
    <strong>Sinal Analógico:</strong> Uma forma de onda contínua cujas características
    físicas (como formato, amplitude e frequência) representam outra dimensão física
    (ex: o sinal elétrico de um microfone representa a variação da pressão do som
    no ar).
  </li>
  <li>
    <strong>Sinal Digital:</strong> Composto por apenas dois níveis (matematicamente
    0 ou 1; fisicamente representado por ligado/desligado ou presença/ausência de
    corrente ou luz).
  </li>
</ul>

<p>
  Os microprocessadores trabalham exclusivamente com dados digitais, tornando
  necessários os conversores:
</p>

<ul>
  <li>
    <strong>Conversor Analógico-Digital (AD):</strong> Retalha o sinal analógico
    em pequenos intervalos de tempo, quantiza cada pedaço e gera uma representação
    binária (digital).
  </li>
  <li>
    <strong>Conversor Digital-Analógico (DA):</strong> Realiza o processo inverso,
    criando um sinal analógico (geralmente uma tensão contínua) a partir de informações
    binárias.
  </li>
  <li>
    <strong>Exemplo do texto:</strong> As placas de som usam o conversor AD para
    a entrada de áudio do microfone e o conversor DA para a saída de áudio dos fones
    de ouvido.
  </li>
</ul>

<p>
  Outros periféricos comuns incluem <strong>timers</strong> (que marcam
  intervalos de tempo),
  <strong>sensores</strong> e <strong>botões</strong>.
</p>

<h3>Microcontroladores</h3>

<p>
  Os microcontroladores são circuitos integrados que possuem, em um mesmo
  encapsulamento, o microprocessador e uma série de periféricos integrados. Eles
  são compostos por uma CPU conectada à memória e aos dispositivos de entrada e
  saída por meio de <strong>barramentos</strong> (bus).
</p>

<ul>
  <li>
    <strong>Barramentos:</strong> Vias de condutores elétricos internos que transportam
    instruções, dados e controle.
  </li>
  <li>
    <strong>Classificação por bits:</strong> O número de bits de um microcontrolador
    determina a quantidade de condutores de cada barramento.
  </li>
</ul>

<h3>Exemplos de Dispositivos</h3>

<p>
  Até o final dos anos 1990, era comum o uso de microprocessadores e periféricos
  em chips separados, montados em placas de circuito impresso grandes.
  Gradativamente, eles foram substituídos por microcontroladores, que se
  tornaram mais especializados e baratos.
</p>

<h3>Microprocessador Z80</h3>

<p>
  Projetado e lançado pela empresa Zilog em 1976, o Z80 foi um dos
  microprocessadores mais populares de todos os tempos, sendo amplamente clonado
  entre os anos 1980 e 2000. Foi utilizado tanto em sistemas embarcados quanto
  em computadores pessoais.
</p>

<h4>Principais aplicações:</h4>

<ul>
  <li>Computadores pessoais (como o Commodore 128).</li>
  <li>Calculadoras gráficas da Texas Instruments.</li>
  <li>Placas de arcade e videogames (Master System, Mega Drive e Game Boy).</li>
  <li>Modelos de MP3 players dedicados.</li>
</ul>

<h3>Microcontroladores 8051 e PIC</h3>

<p>
  A partir dos anos 1990, os microcontroladores cresceram em capacidade,
  famílias e modelos.
</p>

<h4>Microcontrolador 8051</h4>

<p>
  Desenvolvido pela Intel em meados dos anos 1980, é um dos mais populares do
  mercado e possui milhares de clones e variantes.
</p>

<ul>
  <li>
    <strong>Programação:</strong> Suporta Assembly (com conjunto de 16 instruções
    focadas em bits e pouca abstração) e C.
  </li>
  <li>
    <strong>Recursos internos:</strong> Memória RAM, memória de dados EEPROM, interrupções,
    comunicação serial, timers e 4 portas de entrada/saída (E/S).
  </li>
  <li>
    <strong>Operação:</strong> Requer um circuito de clock externo composto por dois
    capacitores e um cristal de quartzo.
  </li>
</ul>

<h4>Família PIC (Programmable Interface Controller)</h4>

<p>
  Desenvolvida pela Microchip Technology desde meados dos anos 1970. Pode ser
  programada em C ou Assembly (cujo conjunto de instruções difere do assembly do
  8051). Exemplos de modelos da família:
</p>

<ul>
  <li>
    <strong>PIC16F84:</strong> Possui baixo consumo de energia, larga faixa de tensão
    de operação, timer interno e controles de E/S.
  </li>
  <li>
    <strong>PIC16F877:</strong> Possui 5 conjuntos de portas de E/S, conversor analógico-digital
    (10 bits de resolução e 8 canais de entrada), periférico de comunicação paralela
    e serial, 2 módulos de comparação, captura e PWM, além de 3 timers.
  </li>
</ul>

<h3>Plataforma de Prototipagem Arduino</h3>

<p>
  Desenvolvido na Itália na metade dos anos 2000, o Arduino é uma plataforma
  simplificada voltada para pequenos projetos educacionais de baixo custo. É
  baseado em licenças livres (LGPL/GPL para software e Creative Commons para
  hardware), o que permite a cópia e a criação de clones (como o Pinguino,
  baseado em microcontrolador PIC).
</p>

<h4>Características da plataforma:</h4>

<ul>
  <li>
    Composta por um microcontrolador Atmel AVR, circuito de clock, pinos de
    entrada/saída digital e analógica e interface USB.
  </li>
  <li>Modelos populares incluem o Arduino UNO e o Arduino MEGA.</li>
  <li><strong>Programação:</strong> Realizada na linguagem C.</li>
  <li>
    <strong>Shields:</strong> Módulos expansivos que se conectam à placa para adicionar
    funções como redes sem fio, controle de motores elétricos ou sensores.
  </li>
</ul>

<h3>Programação de Microcontroladores</h3>

<p>
  Os microcontroladores são comumente programados em Assembly ou C. O exemplo
  padrão para iniciar os estudos nessa área é o circuito "Pisca-Pisca"
  (equivalente ao "Olá, mundo!" dos computadores), que consiste em fazer um LED
  piscar. Diferente dos programas de computadores convencionais, que possuem um
  fim determinado, os programas para sistemas embarcados rodam em um laço
  contínuo (loop infinito), pois devem permanecer em funcionamento constante na
  aplicação.
</p>

<h3>Circuito e Lógica de Funcionamento</h3>

<p>
  Como a tensão dos microcontroladores comerciais geralmente é de 5 V, o LED é
  ligado a um pino da Unidade Microcontroladora (MCU) em série com um resistor
  (na faixa de 100 Ω) para limitação de corrente. A lógica descrita pelo
  fluxograma segue estas etapas em ciclo infinito:
</p>

<ol>
  <li>Configurar um pino do microcontrolador como saída.</li>
  <li>Acender o LED (elevar a tensão no pino para 5 V).</li>
  <li>Esperar 1 segundo.</li>
  <li>Apagar o LED (zerar a tensão no pino).</li>
  <li>Esperar 1 segundo e retornar ao passo 2.</li>
</ol>

<h3>Programação em Assembly</h3>

<p>
  A linguagem Assembly opera com baixo nível de abstração e depende diretamente
  das especificações contidas no manual técnico (datasheet) de cada componente.
</p>

<h4>Assembly para o 8051</h4>

<ul>
  <li>
    Os comentários no código são inseridos após o caractere ponto e vírgula (;).
  </li>
  <li>
    Não possui estruturas condicionais ou de repetição convencionais (como if,
    for ou while); essas ações são simuladas com seu conjunto de instruções
    básicas.
  </li>
  <li>
    Não possui instruções nativas de atraso de tempo. O atraso precisa ser
    implementado manualmente via código, o que costuma consumir cerca de metade
    das linhas do programa.
  </li>
  <li>No exemplo, o LED é conectado ao pino 0 da porta 1 (P1.0).</li>
</ul>

<h4>Assembly para o PIC 16F877</h4>

<ul>
  <li>
    Apresenta um preâmbulo extenso para a inclusão de bibliotecas e
    configurações de funções do chip.
  </li>
  <li>
    Assim como no 8051, não há comandos prontos para atraso de tempo ou
    estruturas de controle (if, for, etc.), exigindo construção manual de cada
    ação.
  </li>
  <li>No exemplo, o LED é conectado ao pino 0 da porta B (RB0).</li>
</ul>

<h3>Programação em C</h3>

<p>
  A linguagem C oferece maior abstração, facilitando a escrita e a compreensão
  do código.
</p>

<h4>C para o PIC 16F877</h4>

<ul>
  <li>
    Possui um preâmbulo inicial característico para definições do sistema.
  </li>
  <li>
    As instruções de atraso de tempo já estão inclusas nas bibliotecas nativas
    do compilador do microcontrolador, dispensando a criação manual de rotinas
    de tempo.
  </li>
  <li>O LED também é mapeado para o pino 0 da porta B (RB0).</li>
</ul>

<h4>C para a Plataforma Arduino</h4>

<ul>
  <li>
    O código é ainda mais simplificado e reduzido em comparação ao C tradicional
    de outros microcontroladores.
  </li>
  <li>
    No exemplo prático dessa plataforma, o LED utiliza o pino 13, cuja numeração
    é identificada diretamente na placa.
  </li>
</ul>

<h3>Aplicações dos Sistemas Embarcados</h3>

<p>
  Os microcontroladores estão presentes em uma enorme variedade de dispositivos
  atuais, automatizando funções e facilitando as tarefas do dia a dia em
  diferentes setores.
</p>

<h4>Uso Residencial e Eletrodomésticos</h4>

<p>
  Os microcontroladores são integrados a aparelhos domésticos sempre que há
  necessidade de controle de tempo ou de funções específicas.
</p>

<ul>
  <li>
    <strong>Fornos de micro-ondas:</strong> Utilizam microcontroladores visíveis
    no painel, operando com periféricos como teclado e display numérico para executar
    seus algoritmos de aquecimento.
  </li>
  <li>
    <strong>Máquinas de lavar:</strong> Gerenciam sistemas programáveis que definem
    e controlam o tempo de molho, lavagem, centrifugação e secagem de acordo com
    o tipo de roupa.
  </li>
  <li>
    <strong>Periféricos e Entretenimento:</strong> Estão presentes nos controles
    de videogames (joypads), em roteadores de internet e em impressoras (para comunicação
    com o computador, controle de motores de papel e emissão de tinta).
  </li>
</ul>

<h4>Automação Industrial e Robótica</h4>

<p>
  A indústria utiliza a construção em massa de placas dedicadas e a programação
  de microcontroladores para criar sistemas de controle específicos.
</p>

<ul>
  <li>
    <strong>Automação Industrial:</strong> Baseia-se no desenvolvimento de sistemas
    dedicados a tarefas específicas auxiliados por uma grande quantidade de sensores.
  </li>
  <li>
    <strong>Robótica:</strong> Um segmento especializado dentro da automação industrial
    que representa uma das grandes revoluções tecnológicas atuais.
  </li>
</ul>

<h4>Automação Residencial (Domótica)</h4>

<p>
  Embora o gerenciamento central e os comandos de voz utilizem plataformas de
  grande porte (como Amazon Alexa, Google ou Apple), o controle final dos
  dispositivos físicos é feito por microcontroladores. Eles realizam o
  processamento de dados e o acionamento de motores ou chaves eletrônicas em:
</p>

<ul>
  <li>Interruptores automáticos por comando de voz.</li>
  <li>
    Lâmpadas inteligentes com acendimento automático e iluminação programável.
  </li>
  <li>Controles remotos de portões.</li>
  <li>Fechaduras biométricas ou com senha.</li>
  <li>Controles de persianas e janelas.</li>
  <li>Sistemas de alarme.</li>
</ul>

<h4>Internet das Coisas (IoT)</h4>

<p>
  A Internet das Coisas é uma vertente da automação viabilizada diretamente pelo
  avanço dos microcontroladores, consistindo na conectividade e coleta de dados
  em tempo real em diversos setores:
</p>

<ul>
  <li>
    <strong>Sistemas Vestíveis (Wearables):</strong> Dispositivos acoplados a roupas,
    relógios e bonés voltados para sensoriamento e análise de dados.
  </li>
  <li>
    <strong>Saúde:</strong> Aplicação em monitores cardíacos, medidores de glicose
    e equipamentos cirúrgicos.
  </li>
  <li>
    <strong>Agricultura:</strong> Sistemas automatizados de plantio, gerenciamento
    e colheita operados sem a necessidade de interação humana direta.
  </li>
</ul>

<h4>Drones</h4>

<p>
  Os drones são dispositivos microcontrolados aplicáveis a todas as áreas
  mencionadas anteriormente, consolidando-se como ferramentas reais para o
  usuário final e apresentando potencial para o futuro dos transportes urbanos e
  das entregas.
</p>

<h3>Conclusão: Conceitos-Chave</h3>

<p>
  Esta etapa sintetizou os fundamentos dos circuitos integrados dedicados ao
  processamento de programas específicos e suas aplicações no cotidiano.
</p>

<h4>Microprocessadores vs. Microcontroladores</h4>

<p>
  Ambos são circuitos integrados (chips) projetados para processar instruções e
  programas particularizados:
</p>

<ul>
  <li>
    <strong>Microprocessadores:</strong> Focam essencialmente no processamento de
    dados e tomadas de decisão.
  </li>
  <li>
    <strong>Microcontroladores:</strong> Integram, em um único chip, a CPU, a memória
    de programas e múltiplos periféricos para viabilizar diferentes tipos de uso.
  </li>
</ul>

<h4>Principais Dispositivos Estudados</h4>

<p>O conteúdo destacou exemplos históricos e práticos dessas tecnologias:</p>

<ul>
  <li>
    <strong>Z80:</strong> Um microprocessador de grande sucesso e ampla utilização
    entre as décadas de 1970 e 1990.
  </li>
  <li>
    <strong>8051 e Família PIC:</strong> Microcontroladores populares que
    oferecem suporte para programação tanto em linguagem de baixo nível (<strong
      >Assembly</strong
    >) quanto em linguagem de alto nível (<strong>C</strong>).
  </li>
  <li>
    <strong>Arduino:</strong> Uma plataforma microcontrolada voltada para prototipagem,
    caracterizada pelo fácil acesso e simplicidade de programação.
  </li>
</ul>

<h4>Aplicações dos Sistemas Embarcados</h4>

<p>
  Os sistemas embarcados possuem uma abrangência gigantesca no mercado atual.
  Eles operam de forma invisível ou explícita em uma vasta gama de contextos,
  que se estendem desde eletrodomésticos de uso doméstico até dispositivos
  tecnológicos avançados e conectados.
</p>
