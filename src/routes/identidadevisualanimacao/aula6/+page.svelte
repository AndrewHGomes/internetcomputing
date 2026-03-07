<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Definição de Realidade Virtual (RV)</h2>

<Audios modulo="M7" aulas={["21", "22", "23", "24"]} />

<p>
  A Realidade Virtual é uma interface avançada que permite ao usuário interagir
  com ambientes tridimensionais gerados por computador em tempo real. Sua
  principal característica é o uso dos sentidos (especialmente a visão) para
  permitir a navegação e a manipulação de objetos em um mundo sintético.
</p>

<ul>
  <li>
    <strong>Virtual:</strong> Representa uma criação computacional ou algo que existe
    como possibilidade, sem efeito material.
  </li>
  <li>
    <strong>Real:</strong> Aquilo que existe concretamente no mundo dos sentidos;
    objetivo.
  </li>
</ul>

<p>
  O objetivo central da RV é substituir a percepção do mundo físico pelos
  sentidos do usuário, voltando-os exclusivamente para o ambiente virtual.
</p>

<h3>O Contínuo de Milgram</h3>

<p>
  Para compreender a relação entre o físico e o digital, utiliza-se o conceito
  de <strong>"Contínuo realidade-virtualidade"</strong>, que organiza as
  tecnologias de acordo com o nível de inserção de elementos virtuais:
</p>

<ul>
  <li>
    <strong>Ambiente Real (Extremidade Esquerda):</strong> O mundo físico sem interferências
    digitais.
  </li>
  <li>
    <strong>Realidade Aumentada (RA):</strong> O usuário permanece no mundo real,
    mas interage com elementos virtuais registrados no espaço físico.
  </li>
  <li>
    <strong>Virtualidade Aumentada (VA):</strong> O usuário é inserido em um ambiente
    virtual que contém elementos capturados do mundo real.
  </li>
  <li>
    <strong>Realidade Virtual (RV) (Extremidade Direita):</strong> Imersão total
    em um ambiente puramente sintético.
  </li>
  <li>
    <strong>Realidade Misturada (RM):</strong> Termo genérico que engloba qualquer
    tecnologia que mescle o real e o virtual (RA e VA).
  </li>
</ul>

<h4>Diferenciação Prática</h4>

<p>
  Embora os limites entre esses conceitos possam ser tênues na prática, a
  distinção fundamental reside na proporção de elementos reais e virtuais:
</p>

<ul>
  <li>A <strong>RV</strong> isola o usuário do mundo físico.</li>
  <li>
    A <strong>RA</strong> sobrepõe o virtual ao físico, mantendo a percepção do entorno
    real.
  </li>
</ul>

<h3>Imersão, Presença e Arquitetura de Sistemas</h3>

<p>
  No âmbito da RV, a distinção entre imersão e presença é fundamental: a
  primeira refere-se às capacidades técnicas do sistema, enquanto a segunda
  trata da experiência psicológica do usuário.
</p>

<h4>Imersão e Presença</h4>

<ul>
  <li>
    <strong>Imersão (Objetiva):</strong> É o nível técnico de precisão com que o
    sistema envia estímulos aos sentidos do usuário. É definida por variáveis
    mensuráveis como:
    <ul>
      <li>
        <strong>Qualidade da imagem:</strong> Resolução e detalhamento de texturas.
      </li>
      <li>
        <strong>Campo de visão e Estereoscopia:</strong> Amplitude do que se vê e
        sensação de profundidade.
      </li>
      <li>
        <strong>Rastreamento:</strong> Precisão e tempo de resposta aos movimentos
        do usuário.
      </li>
      <li>
        <strong>Abrangência e Vivacidade:</strong> Quantidade de sentidos estimulados
        e fidelidade da simulação.
      </li>
      <li>
        <strong>Interatividade e Enredo:</strong> Capacidade de interferir no mundo
        e qualidade da narrativa.
      </li>
    </ul>
  </li>
  <li>
    <strong>Presença (Subjetiva):</strong> É o estado de consciência ou
    percepção psicológica de "estar lá". Ocorre quando o usuário ignora a
    mediação tecnológica. Divide-se em quatro ilusões:
    <ul>
      <li><strong>Espacial:</strong> Sentir-se em um local específico.</li>
      <li>
        <strong>Corporal:</strong> Sentir a existência de um corpo no ambiente virtual.
      </li>
      <li>
        <strong>Física:</strong> Sentir que pode interagir com os objetos do cenário.
      </li>
      <li>
        <strong>Social:</strong> Sentir que pode se comunicar com outros personagens.
      </li>
    </ul>
  </li>
</ul>

<h4>Arquitetura de Sistemas e Processamento</h4>

<p>
  O sistema de RV funciona como um ciclo contínuo de entrada, processamento e
  resposta:
</p>

<ol>
  <li>
    <strong>Interface e Entrada:</strong> O usuário interage via sensores e dispositivos
    de entrada.
  </li>
  <li>
    <strong>Simulação:</strong> É o núcleo do sistema. Cruza os dados de entrada
    com a base de dados para atualizar eventos e animações.
  </li>
  <li>
    <strong>Renderização Sensorial:</strong> Traduz o processamento da máquina em
    estímulos para o usuário, realimentando o sistema.
  </li>
</ol>

<h4>Latência e Desempenho</h4>

<ul>
  <li>
    <strong>Tempo de Latência:</strong> É o intervalo entre a ação do usuário e
    a resposta visual. Deve ser menor que <strong>20ms</strong> para evitar desconforto
    (cinetose) e manter a sensação de presença.
  </li>
  <li>
    <strong>Técnicas de Otimização:</strong> Para reduzir a latência, utilizam-se
    métodos como o Timewarp (reaproveitamento de quadros), aumento da taxa de atualização
    de pixels, otimização da GPU e previsão de movimento da cabeça.
  </li>
</ul>

<h3>Recursos, Interação e Aplicações da RV</h3>

<p>
  O sistema de Realidade Virtual é composto por um ecossistema de hardware e
  software que trabalha em paralelo para reduzir a latência e processar
  múltiplas tarefas, como rastreamento, áudio, simulação física e gestão de
  dispositivos.
</p>

<h4>Interação do Usuário</h4>

<p>
  A interação em ambientes virtuais é dividida em quatro pilares fundamentais:
</p>

<ul>
  <li>
    <strong>Navegação:</strong> Composta pela <strong>viagem</strong>
    (movimentação mecânica) e pelo
    <strong>trajeto</strong> (processo cognitivo de orientação).
  </li>
  <li>
    <strong>Seleção:</strong> Processo de escolher um objeto através da indicação,
    confirmação e realimentação sensorial.
  </li>
  <li>
    <strong>Manipulação:</strong> Alteração das propriedades do objeto, como posição,
    rotação, escala ou cor.
  </li>
  <li>
    <strong>Controle do Sistema:</strong> Envio de comandos via menus, voz ou gestos.
  </li>
</ul>

<h4>Desafios Tecnológicos e Psicológicos</h4>

<ul>
  <li>
    <strong>Vale da Estranheza (Uncanny Valley):</strong> Fenômeno em que representações
    humanas quase perfeitas, mas não idênticas ao real, causam repulsa ou desconforto
    no usuário. Uma solução comum é adotar estilos mais cartunescos e menos fotorrealistas.
  </li>
  <li>
    <strong>Fidelidade:</strong> O alto custo para atingir o fotorrealismo nem
    sempre garante uma experiência satisfatória. A eficácia depende da qualidade
    da <strong>representação</strong>
    (visual), da <strong>interação</strong> (física) e da
    <strong>experiência</strong> (sensação de realidade).
  </li>
</ul>

<h4>Áreas de Aplicação</h4>

<p>
  A RV transcende o entretenimento, sendo aplicada em diversos setores
  estratégicos:
</p>

<ul>
  <li>
    <strong>Indústria:</strong> Uso de CAD 3D, prototipagem virtual, simulação de
    linhas de montagem e testes em túneis de vento digitais.
  </li>
  <li>
    <strong>Saúde:</strong> Planejamento de cirurgias complexas, processamento de
    tomografias 3D e reabilitação de pacientes.
  </li>
  <li>
    <strong>Ciência:</strong> Visualização de dados abstratos, exploração de superfícies
    planetárias e simulação de estruturas atômicas ou moleculares.
  </li>
  <li>
    <strong>Educação:</strong> Laboratórios virtuais, bibliotecas interativas e ambientes
    de aprendizagem colaborativa remota.
  </li>
  <li>
    <strong>Artes e Entretenimento:</strong> Museus virtuais, criação de esculturas
    digitais, cinema imersivo e jogos.
  </li>
</ul>

<h3>Realidade Aumentada (RA)</h3>

<p>
  Diferente da Realidade Virtual, que isola o usuário em um mundo sintético, a
  Realidade Aumentada transporta elementos virtuais para o espaço físico. O
  objetivo é enriquecer o ambiente real com objetos sintetizados, permitindo a
  coexistência e interação simultânea entre ambos.
</p>

<h4>Funcionamento e Requisitos Técnicos</h4>

<p>
  A RA exige que o sistema reconheça o ambiente e o ponto de vista do usuário em
  tempo real para posicionar os objetos virtuais corretamente.
</p>

<ul>
  <li>
    <strong>Rastreamento (Tracking):</strong> Conceito-chave que identifica a posição
    e o formato de exibição do objeto virtual conforme o movimento do observador.
  </li>
  <li>
    <strong>Dispositivos:</strong> Utiliza smartphones, tablets ou óculos especiais
    (HMDs) com câmeras.
  </li>
  <li>
    <strong>Latência:</strong> Para ser considerada "tempo real" e evitar falhas
    de registro, a latência deve ser de no máximo <strong>100ms</strong>.
  </li>
  <li>
    <strong>Interface Multimodal:</strong> Uso combinado de vários dispositivos (mãos,
    voz, sensores) para facilitar a interação.
  </li>
</ul>

<h4>Arquitetura do Sistema de RA</h4>

<p>O processamento é dividido em três módulos principais:</p>

<ol>
  <li>
    <strong>Módulo de Entrada:</strong> Captura de vídeo da cena real e sensoriamento
    (identificação de objetos e posicionamento).
  </li>
  <li>
    <strong>Módulo de Processamento:</strong>
    <ul>
      <li>
        <strong>Monitoramento:</strong> Registro (registering) e rastreamento
        (tracking) do objeto virtual.
        <ul>
          <li>
            <strong>Gerenciamento da Interação:</strong> Responde às ações de seleção
            e manipulação.
          </li>
          <li>
            <strong>Processamento da Aplicação:</strong> Dá sentido às interações
            conforme o objetivo do software.
          </li>
        </ul>
      </li>
    </ul>
  </li>
  <li>
    <strong>Módulo de Saída:</strong> Renderização visual do objeto e atuação em
    dispositivos hápticos (tato).
  </li>
</ol>

<h4>Classificações da Realidade Aumentada</h4>

<p>
  A RA pode ser categorizada pela forma como os dados entram no sistema ou pelo
  tipo de conteúdo exibido:
</p>

<ul>
  <li>
    <strong>Por Rastreamento:</strong>
    <ul>
      <li>
        <strong>Baseada em Visão:</strong> Utiliza o processamento da imagem da câmera
        para reconhecer onde colocar o objeto.
      </li>
      <li>
        <strong>Baseada em Sensores:</strong> Utiliza GPS, giroscópios, acelerômetros
        ou sensores de profundidade.
      </li>
    </ul>
  </li>
  <li>
    <strong>Por Elemento Virtual:</strong>
    <ul>
      <li><strong>1D:</strong> Adição de textos simples (avisos).</li>
      <li><strong>2D:</strong> Gráficos, esquemas ou menus sobrepostos.</li>
      <li>
        <strong>3D:</strong> Objetos tridimensionais realistas integrados ao cenário.
      </li>
    </ul>
  </li>
</ul>

<h4>Ferramentas de Autoria</h4>

<p>
  Atualmente, o <strong>ARToolKit</strong> é uma das bibliotecas de código aberto
  mais populares para o desenvolvimento de RA. Baseado em linguagens como C, C++
  e Java, ele utiliza um sistema de marcadores para facilitar o registro de objetos
  virtuais no mundo físico.
</p>

<h3>Funcionamento da Realidade Aumentada (RA)</h3>

<p>
  A essência da RA reside na capacidade do sistema de identificar onde os
  elementos virtuais devem ser inseridos para que pareçam coexistir com o mundo
  físico. Em elementos 3D, essa integração exige coerência espacial absoluta
  entre o virtual e o real.
</p>

<h4>Monitoramento e Registro</h4>

<p>O sistema opera através de duas tarefas contínuas:</p>

<ul>
  <li>
    <strong>Registro:</strong> Identifica qual elemento virtual deve aparecer e define
    sua posição e orientação relativa no espaço.
  </li>
  <li>
    <strong>Rastreamento (Tracking):</strong> Monitora como o objeto virtual se desloca
    no ambiente em tempo real.
  </li>
</ul>

<p>
  Para viabilizar essas tarefas, utilizam-se frequentemente os <strong>
    marcadores fiduciais
  </strong>. São imagens ou cartões com padrões específicos que o software
  reconhece para calcular a posição e a orientação da câmera em relação ao
  objeto.
</p>

<h4>Visualização e Perspectiva</h4>

<p>
  A forma como o usuário enxerga a RA depende do hardware e do ponto de vista:
</p>

<ul>
  <li>
    <strong>Modos de Visualização:</strong>
    <ul>
      <li>
        <strong>Monitores/Projeção:</strong> Exibição em telas comuns ou projeção
        direta em objetos físicos.
      </li>
      <li>
        <strong>Visada Óptica Direta (Optical See-Through):</strong> Uso de lentes
        semitransparentes (como óculos de RA) que permitem ver o mundo real diretamente
        com sobreposição digital.
      </li>
      <li>
        <strong>Visão de Câmera (Video See-Through):</strong> O usuário vê o mundo
        real indiretamente através de uma filmagem processada em tempo real (como
        na tela de um smartphone).
      </li>
    </ul>
  </li>
  <li>
    <strong>Perspectivas:</strong> Pode ser em <strong>primeira pessoa</strong>
    (câmera na cabeça),
    <strong>segunda pessoa</strong> (câmera voltada para o usuário) ou
    <strong>terceira pessoa</strong> (câmera atrás do usuário).
  </li>
</ul>

<h4>Outros Conceitos no Contínuo Realidade-Virtualidade</h4>

<p>
  Além da RA e RV, existem variações que misturam o físico e o digital de formas
  específicas:
</p>

<ul>
  <li>
    <strong>Realidade Misturada (RM):</strong> Integração profunda entre elementos
    virtuais e o ambiente físico em tempo real.
  </li>
  <li>
    <strong>Virtualidade Aumentada (VA):</strong> Inserção de elementos reais capturados
    em tempo real dentro de um mundo virtual.
  </li>
  <li>
    <strong>Realidade Diminuída (RD):</strong> Remoção digital de objetos ou detalhes
    da cena real.
  </li>
  <li>
    <strong>Hiper Realidade (HR):</strong> Fusão de RV, realidade física, inteligência
    artificial e inteligência humana.
  </li>
  <li>
    <strong>Realidade Cruzada (RC):</strong> Situação em que ações realizadas no
    mundo virtual geram consequências físicas no mundo real.
  </li>
  <li>
    <strong>Virtualidade Pervasiva (VP):</strong> Ambientes virtuais estendidos por
    elementos físicos e sensoriais (como as experiências "4D").
  </li>
</ul>

<h4>Aplicações Práticas</h4>

<p>
  A RA é aplicada em qualquer campo que se beneficie de informações 3D
  sobrepostas à realidade, como:
</p>

<ul>
  <li>Reparos mecânicos e montagem de equipamentos.</li>
  <li>Cirurgias guiadas por computador.</li>
  <li>Design de interiores e arquitetura.</li>
  <li>Educação, treinamentos e guias de museus.</li>
</ul>

<h3>Conclusão: RV e RA</h3>

<p>
  A Realidade Virtual (RV) e a Realidade Aumentada (RA) diferem fundamentalmente
  na origem do ambiente e na percepção do usuário. Enquanto a RV é composta por
  um ambiente totalmente sintético gerado por computador, a RA utiliza o mundo
  real como base, enriquecendo-o com a inserção de objetos virtuais.
</p>

<p>
  Na Realidade Virtual, o sistema detém o controle total sobre a sensação
  visual, isolando o indivíduo da realidade física. Já na Realidade Aumentada, o
  usuário mantém o seu sentido de presença no mundo real, percebendo os
  elementos digitais como acréscimos ao seu entorno imediato. Os mecanismos de
  funcionamento também seguem caminhos distintos:
</p>

<ul>
  <li>
    <strong>Integração na RV:</strong> O foco está em inserir e adaptar o usuário
    dentro de um universo puramente digital.
  </li>
  <li>
    <strong>Integração na RA:</strong> O desafio técnico é combinar e alinhar perfeitamente
    o conteúdo virtual com o espaço físico existente.
  </li>
</ul>
