<script>
  import Audios from "$lib/components/Audios.svelte";
</script>

<h2>Plataformas Multiusuários</h2>

<Audios modulo="M10" aulas={["17", "18", "19", "20"]} />

<p>
  As plataformas multiusuários permitem que diversos indivíduos acessem e
  atualizem um sistema de forma simultânea e em tem real. O desenvolvimento
  dessas aplicações se integra à estrutura padrão de web (front-end, back-end,
  banco de dados e servidores), mas foca na capacidade de operação coletiva ou
  concorrente.
</p>

<h4>Modos de Operação</h4>

<p>Existem duas formas principais de interação nessas plataformas:</p>

<ul>
  <li>
    <strong>Colaborativa:</strong>
    Usuários trabalham juntos, em tempo real ou de forma assíncrona, para criar ou
    modificar um conteúdo comum. O objetivo é a construção conjunta. Um exemplo clássico
    é o Google Drive, onde várias pessoas editam o mesmo documento simultaneamente.
  </li>
  <li>
    <strong>Concorrente:</strong>
    Vários usuários acessam o sistema ao mesmo tempo para utilizar as mesmas funcionalidades
    ou recursos, mas de forma independente. O sistema utiliza controles de acesso
    para evitar conflitos.
  </li>
</ul>

<h4>Controle de Acesso e Exemplos</h4>

<p>
  Na utilização concorrente, o sistema deve garantir a integridade dos dados
  mesmo com acesso simultâneos. No caso de um banco de dados, múltiplos usuários
  podem consultar ou inserir informações sem gerar erros. Já em sistemas de
  reserva de hotéis, a plataforma garante que, embora muitos tentem reservar o
  mesmo quarto, apenas uma transação seja confirmada, evitando a duplicidade.
</p>

<h3>Vantagens, Desafios e Desvantagens</h3>

<p>
  O uso de plataformas multiusuários é amplo, abrangendo desde redes
  corporativas até redes sociais. Embora otimizem o trabalho coletivo, impõem
  exigências de infraestrutura e segurança.
</p>

<h4>Vantagens das Plataformas Multiusuários</h4>

<ul>
  <li>
    <strong>Colaboração e Agilidade:</strong>
    Permite que usuários trabalhem simultaneamente, acelerando o fluxo de tarefas.
  </li>
  <li>
    <strong>Eficiência de Recursos:</strong>
    Compartilhamento de infraestrutura e servidores, evitando gastos com hardware
    dedicado para cada usuário.
  </li>
  <li>
    <strong>Centralização de Dados:</strong>
    Armazenamento centralizado que facilita backups e o acesso remoto de qualquer
    local.
  </li>
  <li>
    <strong>Escalabilidade:</strong>
    Capacidade de expandir o processamento e armazenamento conforme o aumento do
    número de usuários.
  </li>
  <li>
    <strong>Gestão Centralizada:</strong>
    Painéis de controle que permitem aos administradores gerenciar permissões e acessos
    com precisão.
  </li>
  <li>
    <strong>Redução de Custos:</strong>
    Menor investimento em manutenção de hardware e licenciamento individual de software.
  </li>
</ul>

<h4>Desvantagens e Riscos</h4>

<ul>
  <li>
    <strong>Complexidade de Gestão:</strong>
    Exige controle rigoroso de senhas, níveis de acesso e políticas de segurança.
  </li>
  <li>
    <strong>Gargalos de Performance:</strong>
    Risco de lentidão caso o sistema não seja dimensionado para suportar acessos
    simultâneos massivos.
  </li>
  <li>
    <strong>Conflitos de Edição:</strong>
    Possibilidade de erros quando dois usuários alteram o mesmo dado ao mesmo tempo
    sem controle de versão.
  </li>
  <li>
    <strong>Vulnerabilidade:</strong>
    O aumento do número de acessos amplia a superfície de ataque para hackers.
  </li>
  <li>
    <strong>Custos de Manutenção:</strong>
    Embora economize em hardware, exige alto investimento em segurança, monitoramento
    e atualizações constantes.
  </li>
</ul>

<h4>Desfios para o Desenvolvimento</h4>

<p>
  O desenvolvedor de sistemas multiusuários enfrenta desafios técnicos críticos
  para garantir a viabilidade da plataforma:
</p>

<ul>
  <li>
    <strong>Gerenciamento de Acesso:</strong>
    Implementação de criptografia e autenticação multifatorial (MFA) para proteger
    dados sensíveis.
  </li>
  <li>
    <strong>Controle de Alterações:</strong>
    Criação de mecanismos de versionamento para evitar a perda de informações ou
    conflitos de escrita.
  </li>
  <li>
    <strong>Atualização e Performance:</strong>
    Manutenção contínua para correção de vulnerabilidades e otimização do tempo de
    resposta.
  </li>
  <li>
    <strong>Integração de Sistemas:</strong>
    Complexidade técnica ao conectar a plataforma a sistemas externos, como ERPs
    ou orgãos governamentais.
  </li>
  <li>
    <strong>Documentação e Treinamento:</strong>
    Necessidade de guias claros para que os usuários operem o sistema de forma eficiente
    e segura.
  </li>
</ul>

<h3>Frameworks e Bibliotecas</h3>

<p>
  Frameworks e bibliotacas são ferramentas essenciais para otimizar o
  desenvolvimento, permitindo que o programador foque na lógica do sistema em
  vez de tarefas repetitivas ou configurações básicas.
</p>

<h4>Diferença entre Framework e Biblioteca</h4>

<ul>
  <li>
    <strong>Framework:</strong>
    Funciona como uma estrutura predefinida ou um "guia" para o projeto. Ele oferece
    uma base de código com padrões e componentes reutilizáveis, ditando como a aplicação
    deve ser estruturada para reduzir o tempo de desenvolvimento.
  </li>
  <li>
    <strong>Biblioteca:</strong>
    É uma coleção de códigos pre-escritos focada em tarefas específicas. O desenvolvedor
    a utiliza para resolver problemas pontuais e otimizar operações, sem que ela
    controle a estrutura global do projeto.
  </li>
</ul>

<h4>Exemplos de Frameworks (Front-end e Back-end)</h4>

<ul>
  <li>
    <strong>Angular (Front-end):</strong>
    Framework completo mantido pelo Google. Ideal para Sinle Page Application (SPA),
    pois já integra roteamento, formulários e manipulação de dados.
  </li>
  <li>
    <strong>Vue.js (Front-end):</strong>
    Framework progressivo focado na interface de usuário (UI). Sua principal característica
    é a flexibilidade, podendo ser adotado gradualmente em um projeto.
  </li>
  <li>
    <strong>Laravel (Back-end):</strong>
    Framework PHP abrangente que segue o conceito de "baterias inclusas", oferecendo
    nativamente recursos de autenticação, roteamento e banco de dados.
  </li>
  <li>
    <strong>Django (Back-end):</strong>
    Framework Python voltado ao desenvolvimento rápido. Inclui ferramentas de administração
    e ORM (mapeamento objeto-relacional) prontas para uso.
  </li>
</ul>

<h4>React e Node.js</h4>

<ul>
  <li>
    <strong>React:</strong>
    Diferente dos frameworks citados, o React é uma <strong>bibliotaca</strong>
    JavaScript focada exclusivamente na construção de interfaces (UI). Ele lida com
    a renderização de componentes, mas depende de outras bibliotacas para funções
    como roteamento.
  </li>
  <li>
    <strong>Node.js:</strong>
    Não é uma linguagem, mas um <strong>ambiente de execução (runtime)</strong>.
    Ele permite que o JavaScript seja executado no lado do servidor (back-end),
    utilizando o o motor V8 do Chrome para processar os scripts.
  </li>
</ul>

<h3>Instalação do Node.js e Criação de Projeto React</h3>

<p>
  O Node.js é o ambiente necessário para executar JavaScript fora do navegador,
  permitindo o uso de ferramentas de automação e bibliotecas como o React.
</p>

<h4>Passo a Passo: Instalação do Node.js</h4>

<ol>
  <li>
    <strong>Download:</strong> Acesse o site oficial e escolha sempre a versão LTS
    (mais estável).
  </li>
  <li>
    <strong>Instalação:</strong> Execute o instalador, avance as etapas ("Next")
    e marque a opção "Automatically install..." para garantir que as dependências
    complementares sejam configuradas.
  </li>
  <li>
    <strong>Finalização:</strong> Reinicie o computador após concluir o processo.
  </li>
  <li>
    <strong>Verificação:</strong> Abra o prompt de comando (CMD) e digite node --version.
    O sucesso é confirmado se o sistema retornar o número da versão instalada.
  </li>
</ol>

<h4>Criando um Projeto React</h4>

<p>
  Com o Node.js pronto, a criação de uma aplicação React é feita via linha de
  comando:
</p>

<ul>
  <li>
    <strong>Comando de Criação:</strong> Digite npm create vite@latest
    nome-do-projeto -- --template react.
    <ul>
      <li>
        <strong>Nota:</strong> O nome não deve conter espaços ou caracteres especiais.
        Confirme com "y" se solicitado.
      </li>
    </ul>
  </li>
  <li>
    <strong>Navegação:</strong> Entre na pasta criada com o comando cd nome-do-projeto.
  </li>
  <li><strong>Instalar as dependências: </strong> npm install</li>
  <li>
    <strong>Execução:</strong> Digite npm run dev. O projeto será compilado e aberto
    automaticamente no navegador em localhost.
  </li>
</ul>

<h4>Integração com o Visual Studio Code</h4>

<p>Para editar o código de forma profissional, utiliza-se o VS Code:</p>

<ul>
  <li>
    <strong>Abertura Rápida:</strong> Dentro da pasta do projeto no prompt, digite
    code . para abrir o editor diretamente naquele diretório.
  </li>
  <li>
    <strong>Estrutura Pronta:</strong> Ao abrir, o projeto já conterá uma estrutura
    de arquivos e códigos base (boilerplates). Isso permite focar no desenvolvimento
    das funcionalidades, já que as configurações de sintaxe e dependências são gerenciadas
    pela biblioteca.
  </li>
</ul>

<p>
  O foco desse processo é observar a composição e o funcionamento prático de uma
  plataforma web moderna, utilizando ferramentas que automatizam a
  infraestrutura inicial.
</p>

<h3>Conclusão e Prática</h3>

<p>
  Nesta etapa, consolidamos o entendimento sobre a infraestrutura moderna de
  desenvolvimento web e a aplicação prática das ferramentas apresentadas.
</p>

<ul>
  <li>
    <strong>Plataformas Multiusuários:</strong> Compreensão de sistemas que permitem
    interações simultâneas e em tempo real, equilibrando agilidade com desafios de
    segurança e performance.
  </li>
  <li>
    <strong>Ecossistema de Ferramentas:</strong> Diferenciação clara entre
    <strong>Frameworks</strong>
    (estruturas guias), <strong>Bibliotecas</strong> (coleções de funções
    específicas como o React) e <strong>Ambientes de Execução</strong> (como o Node.js).
  </li>
  <li>
    <strong>Agilidade no Desenvolvimento:</strong> Observação de como o uso de bibliotecas
    e ambientes pré-configurados elimina a necessidade de criar sintaxes e configurações
    do zero, acelerando a entrega de projetos.
  </li>
</ul>

<h4>Próximos Passos para Aprofundamento</h4>

<p>
  Para internalizar os conceitos e expandir o conhecimento técnico,
  recomenda-se:
</p>

<ul>
  <li>
    <strong>Exploração do Node.js:</strong> Acessar a documentação oficial (disponível
    em português) para entender melhor como o motor JavaScript processa requisições
    no servidor.
  </li>
  <li>
    <strong>Prática com React:</strong> Analisar os arquivos gerados automaticamente
    na criação do projeto para identificar como a biblioteca organiza os componentes
    da interface.
  </li>
  <li>
    <strong>Estudo de Caso:</strong> Refletir sobre como grandes plataformas (como
    redes sociais ou editores de texto online) gerenciam a colaboração e a concorrência
    discutidas anteriormente.
  </li>
</ul>
