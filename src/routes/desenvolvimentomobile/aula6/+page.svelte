<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>A Necessidade da Persistência de Dados</h2>

<Audios modulo="M9" aulas={["21", "22", "23", "24"]} />

<p>
  Dados armazenados apenas em variáveis de memória (como um array simples) são
  perdidos assim que o aplicativo é fechado ou o sistema operacional o encerra
  para liberar recursos. Para que as informações (como fotos) sobrevivam ao
  fechamento do app, elas precisam ser gravadas fisicamente no armazenamento
  interno do dispositivo (o sistema de arquivos).
</p>

<h3>Fluxo de Salvamento de Mídia</h3>

<p>
  O processo de salvar uma imagem capturada envolve transformar um dado volátil
  em um arquivo permanente. O fluxo lógico seguido é:
</p>

<ol>
  <li>
    <strong>Captura:</strong> O hardware da câmera gera um caminho temporário para
    a imagem.
  </li>
  <li>
    <strong>Conversão:</strong> O dado da imagem é convertido para um formato de
    transferência, como Base64 (uma representação de dados binários em formato de
    texto).
  </li>
  <li>
    <strong>Escrita:</strong> O sistema de arquivos do dispositivo recebe esse dado
    e o grava com um nome único (geralmente baseado no registro de data e hora para
    evitar duplicidade).
  </li>
</ol>

<h3>Tratamento de Dados: Blobs e Base64</h3>

<p>
  No contexto de aplicações que rodam sobre motores web, o tratamento de
  arquivos exige etapas intermediárias de conversão:
</p>

<ul>
  <li>
    <strong>Fetch e Blob:</strong> O aplicativo busca o arquivo temporário da câmera
    e o converte em um Blob (Binary Large Object), que é uma representação bruta
    do arquivo.
  </li>
  <li>
    <strong>FileReader:</strong> Uma ferramenta que lê esse objeto binário e o transforma
    em uma String Base64, permitindo que ele seja facilmente salvo como texto no
    sistema de arquivos ou enviado para um banco de dados.
  </li>
</ul>

<h3>Modularização e Abstração</h3>

<p>
  Uma boa prática de arquitetura destacada é o uso de <strong
    >funções auxiliares</strong
  >
  (métodos privados). Ao isolar a lógica de conversão (readAsBase64) e a lógica de
  salvamento (savePicture), o código principal permanece limpo e focado no objetivo
  do usuário, enquanto a complexidade técnica e as diferenças entre plataformas (Web
  vs. Mobile) ficam protegidas dentro dessas funções específicas.
</p>

<h3>Persistência com Armazenamento Chave-Valor</h3>

<p>
  Para que a lista de fotos apareça sempre que o app for aberto, não basta
  salvar os arquivos de imagem; é preciso salvar a <strong
    >lista de referências</strong
  > (os caminhos dos arquivos).
</p>

<ul>
  <li>
    <strong>API de Preferências:</strong> Utiliza-se um sistema de armazenamento
    simples do tipo chave-valor (como um dicionário).
  </li>
  <li>
    <strong>Serialização JSON:</strong> Como essas APIs geralmente salvam apenas
    texto, a lista de objetos (array) é convertida em uma string JSON para ser armazenada
    e, posteriormente, convertida de volta para objeto ao carregar.
  </li>
</ul>

<h3>Ciclo de Vida: Inicialização</h3>

<p>
  A recuperação dos dados deve ocorrer no momento em que a página é carregada.
  Utiliza-se um evento de ciclo de vida (como o ngOnInit ou similar) para
  disparar a função de carregamento assim que o componente é criado, garantindo
  que o usuário veja sua galeria imediatamente.
</p>

<h3>Desenvolvimento Híbrido e Detecção de Plataforma</h3>

<p>
  O grande diferencial de frameworks modernos é usar o mesmo código para
  diferentes sistemas. No entanto, o acesso a arquivos varia entre a Web e o
  Celular. A estratégia utilizada é a <strong
    >Diferenciação por Plataforma</strong
  >:
</p>

<ul>
  <li>
    <strong>Plataforma Híbrida (iOS/Android):</strong> O app acessa o sistema de
    arquivos nativo diretamente. Os caminhos de arquivo (URIs) precisam ser convertidos
    para um formato que a visualização do app consiga entender.
  </li>
  <li>
    <strong>Plataforma Web:</strong> O navegador exige que os arquivos sejam lidos
    e convertidos para o formato Base64 para serem exibidos como imagens.
  </li>
</ul>

<h4>Resumo das Adaptações Técnicas:</h4>

<ul>
  <li>
    <strong>Leitura de Arquivo:</strong> No celular, o arquivo é lido diretamente
    do caminho nativo; na web, ele é buscado e convertido.
  </li>
  <li>
    <strong>Exibição de Imagem:</strong> No celular, usa-se uma função de conversão
    de fonte (ex: convertFileSrc) para mapear o arquivo local; na web, usa-se a string
    Base64 ou o caminho temporário.
  </li>
</ul>

<h4>Fluxo</h4>

<p>
  Ao implementar essas verificações, o serviço torna-se inteligente: ele detecta
  onde está rodando e escolhe o método mais eficiente para salvar e carregar as
  fotos. Com isso, o projeto está pronto para a <strong
    >implantação (deploy)</strong
  >, saindo do ambiente de testes e indo para o hardware real.
</p>

<h3>O Papel do Runtime Nativo</h3>

<p>
  Para que uma aplicação web funcione como um aplicativo nativo, utiliza-se um
  <strong>Runtime</strong> (como o Capacitor ou o antigo Cordova). Ele atua como
  uma ponte que envolve o código web (HTML/JS/CSS) e permite que ele seja executado
  dentro de um "contêiner" nativo no Android ou iOS, acessando as APIs do sistema
  operacional.
</p>

<h4>Fluxo de Preparação e Sincronização</h4>

<p>
  O processo de transformar o código-fonte em um aplicativo distribuível segue
  etapas rigorosas:
</p>

<ul>
  <li>
    <strong>Build:</strong> O comando de compilação gera os arquivos estáticos finais
    (geralmente em uma pasta www ou dist).
  </li>
  <li>
    <strong>Adição de Plataformas:</strong> Cria-se as pastas de projeto específicas
    para cada sistema operacional (Android/iOS). Estes são projetos nativos reais
    que podem ser abertos em IDEs como Android Studio ou Xcode.
  </li>
  <li>
    <strong>Cópia e Sincronização:</strong> Sempre que o código web é alterado, as
    mudanças devem ser copiadas para as pastas nativas (copy). Se houver novos plugins
    ou permissões, utiliza-se o comando de sincronização (sync).
  </li>
</ul>

<h3>Gerenciamento de Permissões Nativa</h3>

<p>
  Diferente da web, dispositivos móveis exigem que as intenções de uso do
  hardware sejam declaradas explicitamente em arquivos de configuração (como o
  AndroidManifest.xml).
</p>

<ul>
  <li>
    <strong>Declaração de Permissões:</strong> O desenvolvedor deve listar que o
    app precisará de acesso à leitura e escrita no armazenamento externo e à câmera.
  </li>
  <li>
    <strong>Consentimento do Usuário:</strong> Além da declaração no código, o sistema
    operacional solicitará a permissão ao usuário na primeira vez que a funcionalidade
    for acionada.
  </li>
</ul>

<h3>Ciclo de Desenvolvimento Final</h3>

<p>O encerramento do ciclo de desenvolvimento consiste em:</p>

<ol>
  <li>Conectar o dispositivo físico ao computador.</li>
  <li>Utilizar a IDE nativa (Android Studio) para compilar o pacote final.</li>
  <li>
    Executar o "Deploy" (instalação) diretamente no hardware para testes de
    desempenho e usabilidade real.
  </li>
</ol>
