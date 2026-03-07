<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Natureza Física do Som</h2>

<Audios modulo="M5" aulas={["13", "14", "15", "16"]} />

<p>
  O som é um elemento onipresente e sutil, cuja importância muitas vezes só é
  notada quando há falhas na captação ou reprodução. Para trabalhar com áudio, é
  fundamental entender seus princípios físicos e como ele se comporta no
  ambiente.
</p>

<h3>Definição e Propagação</h3>

<p>
  Fisicamente, o som é uma <strong>onda mecânica e longitudinal</strong>. Ele
  consiste em uma vibração que se propaga através de meios físicos (ar, água,
  sólidos) por meio da movimentação de moléculas. Por depender de um meio
  material, <strong>o som não se propaga no vácuo</strong>.
</p>

<h4>Propriedades da Onda Sonora</h4>

<p>As três propriedades fundamentais que definem como percebemos o som são:</p>

<ul>
  <li>
    <strong>Velocidade:</strong> Depende do meio de propagação. Materiais mais
    densos e elásticos transmitem o som mais rápido. No ar, a velocidade é de
    aproximadamente
    <strong>340 m/s</strong>, enquanto em sólidos como o ferro, pode ultrapassar
    <strong>5.000 m/s</strong>.
  </li>
  <li>
    <strong>Frequência (Hz):</strong> Define se o som é
    <strong>grave ou agudo</strong>. É medida em Hertz (Hz).
    <ul>
      <li><strong>Sons Graves:</strong> Baixa frequência (poucos Hz).</li>
      <li><strong>Sons Agudos:</strong> Alta frequência (muitos Hz).</li>
      <li>
        <strong>Audição Humana:</strong> O espectro audível para humanos varia
        de
        <strong>20 Hz a 20.000 Hz</strong>.
      </li>
    </ul>
  </li>
  <li>
    <strong>Amplitude:</strong> Refere-se à intensidade da energia da onda. No cotidiano,
    é o que chamamos de volume. Aumentar o volume de um aparelho significa aumentar
    a amplitude da onda sonora.
  </li>
</ul>

<h3>Som Mono vs. Estéreo</h3>

<p>
  A forma como ouvimos sons na natureza é espacial: temos dois ouvidos que
  captam diferenças sonoras, permitindo identificar a direção e a distância das
  fontes. A tecnologia de áudio evoluiu para tentar mimetizar essa experiência
  natural.
</p>

<h4>Som Monofônico (Mono)</h4>

<p>
  É o sistema onde todo o áudio é consolidado em um <strong>único canal</strong
  >. Independentemente de quantas caixas de som existam, todas transmitem
  exatamente o mesmo sinal.
</p>

<ul>
  <li><strong>Origem:</strong> Popularizado pelo fonógrafo e gramofone.</li>
  <li>
    <strong>Característica:</strong> O som parece vir de um único ponto central,
    perdendo a noção de espacialidade da gravação original.
  </li>
</ul>

<h4>Som Estereofônico (Estéreo)</h4>

<p>
  Sistema que utiliza <strong>dois canais independentes</strong> (esquerdo e direito).
  Surgiu comercialmente com os discos de vinil na década de 1960.
</p>

<ul>
  <li>
    <strong>Diferencial:</strong> Permite distribuir instrumentos e vozes entre as
    caixas (ex: guitarra na direita, voz na esquerda).
  </li>
  <li>
    <strong>Impacto:</strong> Proporciona uma experiência muito mais imersiva e fiel
    à realidade, simulando o posicionamento dos músicos no palco.
  </li>
</ul>

<h4>Sistemas de Multicanais e Surround</h4>

<p>
  Com o avanço tecnológico, o áudio passou a utilizar mais do que apenas dois
  canais para envolver o ouvinte completamente:
</p>

<ul>
  <li>
    <strong>Sistemas 5.1 / 7.2:</strong> O primeiro número indica a quantidade de
    caixas de som (fontes de áudio distintas) e o segundo número indica a quantidade
    de subwoofers (caixas dedicadas exclusivamente a frequências graves e vibrações).
  </li>
  <li>
    <strong>Dolby Atmos:</strong> Tecnologia de ponta que adiciona a percepção de
    altura (canais no teto), criando uma "bolha" sonora tridimensional.
  </li>
</ul>

<h3>Captação de Áudio e Microfones</h3>

<p>
  A captação de áudio é o processo de converter ondas sonoras (energia acústica)
  em sinais elétricos. Esse papel é desempenhado pelo <strong>microfone</strong
  >, que utiliza o princípio da indução eletromagnética para transformar
  vibrações (como a voz ou instrumentos) em pulsos elétricos que podem ser
  gravados, amplificados ou processados. A escolha do microfone ideal depende
  diretamente do objetivo da gravação e do ambiente onde ela ocorre.
</p>

<ul>
  <li>
    <strong>Microfones Omnidirecionais:</strong> Captam o som de
    <strong>todas as direções</strong>
    com a mesma sensibilidade. São ideais para registrar sons ambientes (natureza,
    trânsito) ou captar a atmosfera de uma sala com várias pessoas. Não são recomendados
    quando se deseja isolar uma fonte sonora específica.
  </li>
  <li>
    <strong>Microfones Condensadores:</strong> Conhecidos pela alta
    sensibilidade e fidelidade, são perfeitos para
    <strong>estúdios e ambientes controlados</strong>. Capturam detalhes sutis
    da voz humana e instrumentos acústicos. São muito utilizados em podcasts e
    gravações musicais onde se busca um som "natural".
  </li>
  <li>
    <strong>Microfones de Lapela:</strong> Pequenos e discretos, são fixados à
    roupa do locutor. São especialistas em <strong>isolar a voz humana</strong>,
    reduzindo os ruídos do ambiente ao redor. São a escolha padrão para
    entrevistas, vídeos para YouTube e apresentações onde a nitidez da fala é a
    prioridade.
  </li>
</ul>

<h3>Edição com o Audacity</h3>

<p>
  O <strong>Audacity</strong> é uma das ferramentas mais populares para edição de
  áudio por ser gratuita, de código aberto e multiplataforma. Ele permite realizar
  desde cortes simples até mixagens complexas com múltiplas faixas.
</p>

<h4>Interface e Primeiros Passos</h4>

<p>
  Ao abrir um arquivo de áudio (<strong>Arquivo &gt; Abrir</strong>), o programa
  exibe as formas de onda. Se o arquivo for estéreo, você verá duas ondas
  sobrepostas (canal esquerdo e direito); se for mono, apenas uma.
</p>

<h4>Ferramentas Essenciais</h4>

<p>Para editar com precisão, o Audacity oferece ferramentas fundamentais:</p>

<ul>
  <li>
    <strong>Seleção (I):</strong> A ferramenta principal. Você clica e arrasta sobre
    a onda para definir qual trecho será editado, excluído ou terá efeitos aplicados.
  </li>
  <li>
    <strong>Zoom (Lupa):</strong> Essencial para edições detalhadas. Com o zoom,
    você pode visualizar frações de segundo para remover um ruído específico ou um
    erro de fala sem afetar o restante do áudio.
  </li>
  <li>
    <strong>Recortar, Copiar e Colar:</strong> Funcionam como em um editor de texto.
    Você pode reorganizar as partes da sua gravação ou duplicar efeitos sonoros facilmente.
  </li>
</ul>

<h4>Controles de Faixa e Mixagem</h4>

<p>
  No painel lateral de cada faixa de áudio, existem controles que afetam a
  reprodução sem alterar permanentemente a onda:
</p>

<ul>
  <li>
    <strong>Ganho (+/-):</strong> Ajusta o volume daquela trilha específica.
  </li>
  <li>
    <strong>Pan (E/D):</strong> Define o balanço, jogando o som mais para o ouvido
    esquerdo ou direito.
  </li>
  <li>
    <strong>Silenciar (Mute):</strong> Desativa temporariamente a faixa para que
    ela não seja ouvida.
  </li>
  <li>
    <strong>Solo:</strong> Desativa todas as outras faixas, permitindo que você ouça
    apenas a trilha selecionada. Isso é muito útil quando se trabalha com várias
    camadas de áudio (voz, trilha sonora e efeitos).
  </li>
</ul>

<h3>Equalização e Finalização de Áudio</h3>

<p>
  A etapa final do trabalho com som envolve o ajuste fino das frequências e a
  preparação do arquivo para distribuição. No Audacity, o menu <strong
    >Efeitos</strong
  > concentra as ferramentas necessárias para equilibrar volumes e timbres.
</p>

<h4>Ajuste de Frequências e Volume</h4>

<ul>
  <li>
    <strong>Equalizador Gráfico:</strong> Permite manipular o espectro audível
    humano (<strong>20 Hz a 20.000 Hz</strong>). Ao mover as alavancas virtuais
    para cima (aumentar) ou para baixo (diminuir), você ajusta a amplitude de
    frequências específicas.
    <ul>
      <li><strong>Esquerda:</strong> Controla os <strong>graves</strong>.</li>
      <li><strong>Direita:</strong> Controla os <strong>agudos</strong>.</li>
    </ul>
  </li>
  <li>
    <strong>Amplificar:</strong> Utilizado para normalizar trechos desequilibrados.
    Se uma pessoa fala mais baixo que a outra na mesma gravação, você pode selecionar
    apenas o trecho silencioso e aumentar sua amplitude de forma independente.
  </li>
  <li>
    <strong>Graves e Agudos:</strong> Uma versão simplificada do equalizador para
    ajustes rápidos, ideal para tornar vozes muito estridentes mais "encorpadas"
    ou dar clareza a falas abafadas.
  </li>
</ul>

<h4>Salvar vs. Exportar</h4>

<p>
  É crucial entender a diferença entre estas duas ações para não perder seu
  trabalho:
</p>

<ol>
  <li>
    <strong>Salvar Projeto (.aup):</strong> Guarda todo o ambiente de trabalho. Salva
    as múltiplas faixas separadas, os silenciamentos (mutes) e o histórico de edição.
    Use isso enquanto o trabalho não estiver terminado.
  </li>
  <li>
    <strong>Exportar (WAV ou MP3):</strong> Gera o arquivo final que pode ser
    ouvido em qualquer player ou celular.
    <ul>
      <li>
        <strong>WAV:</strong> Áudio sem compressão e de alta fidelidade (ideal para
        backup ou edição posterior).
      </li>
      <li><strong>MP3:</strong> Formato comprimido, ideal para a internet.</li>
    </ul>
  </li>
</ol>

<h4>Qualidade de Exportação (Bitrate)</h4>

<p>
  Ao exportar em MP3, você deve escolher a taxa de bits (Kbps), que define o
  equilíbrio entre qualidade sonora e peso do arquivo:
</p>

<ul>
  <li>
    <strong>Qualidade Padrão (145 - 185 Kbps):</strong> Ideal para arquivos leves.
    Use para áudios que serão compartilhados rapidamente em grupos de WhatsApp ou
    para visualização simples na web onde o espaço de armazenamento é limitado.
  </li>
  <li>
    <strong>Qualidade Extrema (220 - 260 Kbps):</strong> O equilíbrio ideal para
    o profissional. É a escolha certa para programas de rádio, podcasts de alta qualidade
    e trilhas sonoras de vídeos que serão publicados no YouTube ou em redes sociais
    profissionais.
  </li>
  <li>
    <strong>Qualidade Insana (320 Kbps):</strong> O nível máximo do MP3. Recomendado
    para produções musicais onde a fidelidade sonora é essencial, chegando muito
    próximo da qualidade de um CD original.
  </li>
</ul>

<h3>Conclusão</h3>

<p>
  Nesta etapa abordamos o som. Discutimos várias coisas superimportantes a
  respeito do áudio e das maneiras de fazê-lo. Desde a parte física do áudio, as
  questões do estéreo e do mono, até o uso de microfones e finalizamos com a
  manipulação do áudio com o software Audacity. No próximo capítulo falaremos
  sobre a produção de vídeo em um software para isso.
</p>
