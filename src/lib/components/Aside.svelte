<script>
  import { base } from "$app/paths";
  import { slide, fly } from "svelte/transition";
  let { menuAberto = $bindable() } = $props();

  const modulos = [
    {
      nome: "1. Introdução ao Curso",
      aulas: [
        { nome: "Aula 1", link: `${base}/introducao/aula1` },
        { nome: "Aula 2", link: `${base}/introducao/aula2` },
        { nome: "Aula 3", link: `${base}/introducao/aula3` },
        { nome: "Aula 4", link: `${base}/introducao/aula4` },
        { nome: "Aula 5", link: `${base}/introducao/aula5` },
        { nome: "Aula 6", link: `${base}/introducao/aula6` },
      ],
    },
    {
      nome: "2. Lógica de Programação e Algoritmos",
      aulas: [
        { nome: "Aula 1", link: `${base}/logicaprogramacaoalgoritmos/aula1` },
        { nome: "Aula 2", link: `${base}/logicaprogramacaoalgoritmos/aula2` },
        { nome: "Aula 3", link: `${base}/logicaprogramacaoalgoritmos/aula3` },
        { nome: "Aula 4", link: `${base}/logicaprogramacaoalgoritmos/aula4` },
        { nome: "Aula 5", link: `${base}/logicaprogramacaoalgoritmos/aula5` },
        { nome: "Aula 6", link: `${base}/logicaprogramacaoalgoritmos/aula6` },
      ],
    },
    {
      nome: "3. Linguagens de Programação",
      aulas: [
        { nome: "Aula 1", link: `${base}/linguagensprogramacao/aula1` },
        { nome: "Aula 2", link: `${base}/linguagensprogramacao/aula2` },
        { nome: "Aula 3", link: `${base}/linguagensprogramacao/aula3` },
        { nome: "Aula 4", link: `${base}/linguagensprogramacao/aula4` },
        { nome: "Aula 5", link: `${base}/linguagensprogramacao/aula5` },
        { nome: "Aula 6", link: `${base}/linguagensprogramacao/aula6` },
      ],
    },
    {
      nome: "4. Interface Web",
      aulas: [
        { nome: "Aula 1", link: `${base}/interfaceweb/aula1` },
        { nome: "Aula 2", link: `${base}/interfaceweb/aula2` },
        { nome: "Aula 3", link: `${base}/interfaceweb/aula3` },
        { nome: "Aula 4", link: `${base}/interfaceweb/aula4` },
        { nome: "Aula 5", link: `${base}/interfaceweb/aula5` },
        { nome: "Aula 6", link: `${base}/interfaceweb/aula6` },
      ],
    },
    {
      nome: "5. Princípios de Web Design",
      aulas: [
        { nome: "Aula 1", link: `${base}/principioswebdesign/aula1` },
        { nome: "Aula 2", link: `${base}/principioswebdesign/aula2` },
        { nome: "Aula 3", link: `${base}/principioswebdesign/aula3` },
        { nome: "Aula 4", link: `${base}/principioswebdesign/aula4` },
        { nome: "Aula 5", link: `${base}/principioswebdesign/aula5` },
        { nome: "Aula 6", link: `${base}/principioswebdesign/aula6` },
      ],
    },
    {
      nome: "6. Projeto Web, Criação e Editoração",
      aulas: [
        { nome: "Aula 1", link: `${base}/projetocriacaoeditoracao/aula1` },
        { nome: "Aula 2", link: `${base}/projetocriacaoeditoracao/aula2` },
        { nome: "Aula 3", link: `${base}/projetocriacaoeditoracao/aula3` },
        { nome: "Aula 4", link: `${base}/projetocriacaoeditoracao/aula4` },
        { nome: "Aula 5", link: `${base}/projetocriacaoeditoracao/aula5` },
        { nome: "Aula 6", link: `${base}/projetocriacaoeditoracao/aula6` },
      ],
    },
    {
      nome: "7. Identidade Visual e Animação",
      aulas: [
        { nome: "Aula 1", link: `${base}/identidadevisualanimacao/aula1` },
        { nome: "Aula 2", link: `${base}/identidadevisualanimacao/aula2` },
        { nome: "Aula 3", link: `${base}/identidadevisualanimacao/aula3` },
        { nome: "Aula 4", link: `${base}/identidadevisualanimacao/aula4` },
        { nome: "Aula 5", link: `${base}/identidadevisualanimacao/aula5` },
        { nome: "Aula 6", link: `${base}/identidadevisualanimacao/aula6` },
      ],
    },
    {
      nome: "8. Plataformas Web",
      aulas: [
        { nome: "Aula 1", link: `${base}/plataformasweb/aula1` },
        { nome: "Aula 2", link: `${base}/plataformasweb/aula2` },
        { nome: "Aula 3", link: `${base}/plataformasweb/aula3` },
        { nome: "Aula 4", link: `${base}/plataformasweb/aula4` },
        { nome: "Aula 5", link: `${base}/plataformasweb/aula5` },
        { nome: "Aula 6", link: `${base}/plataformasweb/aula6` },
      ],
    },
    {
      nome: "9. Estrutura de Bancos de Dados",
      aulas: [
        { nome: "Aula 1", link: `${base}/estruturabancosdados/aula1` },
        { nome: "Aula 2", link: `${base}/estruturabancosdados/aula2` },
        { nome: "Aula 3", link: `${base}/estruturabancosdados/aula3` },
        { nome: "Aula 4", link: `${base}/estruturabancosdados/aula4` },
        { nome: "Aula 5", link: `${base}/estruturabancosdados/aula5` },
        { nome: "Aula 6", link: `${base}/estruturabancosdados/aula6` },
      ],
    },
    {
      nome: "10. Desenvolvimento de Sistemas",
      aulas: [
        { nome: "Aula 1", link: `${base}/desenvolvimentosistemas/aula1` },
        { nome: "Aula 2", link: `${base}/desenvolvimentosistemas/aula2` },
        { nome: "Aula 3", link: `${base}/desenvolvimentosistemas/aula3` },
        { nome: "Aula 4", link: `${base}/desenvolvimentosistemas/aula4` },
        { nome: "Aula 5", link: `${base}/desenvolvimentosistemas/aula5` },
        { nome: "Aula 6", link: `${base}/desenvolvimentosistemas/aula6` },
      ],
    },
    {
      nome: "11. Modelagem de Sistemas Web",
      aulas: [
        { nome: "Aula 1", link: `${base}/modelagemsistemasweb/aula1` },
        { nome: "Aula 2", link: `${base}/modelagemsistemasweb/aula2` },
        { nome: "Aula 3", link: `${base}/modelagemsistemasweb/aula3` },
        { nome: "Aula 4", link: `${base}/modelagemsistemasweb/aula4` },
        { nome: "Aula 5", link: `${base}/modelagemsistemasweb/aula5` },
        { nome: "Aula 6", link: `${base}/modelagemsistemasweb/aula6` },
      ],
    },
    {
      nome: "12. Administração e Sistemas",
      aulas: [
        { nome: "Aula 1", link: `${base}/administracaosistemas/aula1` },
        { nome: "Aula 2", link: `${base}/administracaosistemas/aula2` },
        { nome: "Aula 3", link: `${base}/administracaosistemas/aula3` },
        { nome: "Aula 4", link: `${base}/administracaosistemas/aula4` },
        { nome: "Aula 5", link: `${base}/administracaosistemas/aula5` },
        { nome: "Aula 6", link: `${base}/administracaosistemas/aula6` },
      ],
    },
    {
      nome: "13. Sistemas e Mapeamento de Processos",
      aulas: [
        { nome: "Aula 1", link: `${base}/sistemasmapaeamentoprocessos/aula1` },
        { nome: "Aula 2", link: `${base}/sistemasmapaeamentoprocessos/aula2` },
        { nome: "Aula 3", link: `${base}/sistemasmapaeamentoprocessos/aula3` },
        { nome: "Aula 4", link: `${base}/sistemasmapaeamentoprocessos/aula4` },
        { nome: "Aula 5", link: `${base}/sistemasmapaeamentoprocessos/aula5` },
        { nome: "Aula 6", link: `${base}/sistemasmapaeamentoprocessos/aula6` },
      ],
    },
    {
      nome: "14. Gestão da Informação",
      aulas: [
        { nome: "Aula 1", link: `${base}/gestaoinformacao/aula1` },
        { nome: "Aula 2", link: `${base}/gestaoinformacao/aula2` },
        { nome: "Aula 3", link: `${base}/gestaoinformacao/aula3` },
        { nome: "Aula 4", link: `${base}/gestaoinformacao/aula4` },
        { nome: "Aula 5", link: `${base}/gestaoinformacao/aula5` },
        { nome: "Aula 6", link: `${base}/gestaoinformacao/aula6` },
      ],
    },
    {
      nome: "15. Desenvolvimento Mobile",
      aulas: [
        { nome: "Aula 1", link: `${base}/desenvolvimentomobile/aula1` },
        { nome: "Aula 2", link: `${base}/desenvolvimentomobile/aula2` },
        { nome: "Aula 3", link: `${base}/desenvolvimentomobile/aula3` },
        { nome: "Aula 4", link: `${base}/desenvolvimentomobile/aula4` },
        { nome: "Aula 5", link: `${base}/desenvolvimentomobile/aula5` },
        { nome: "Aula 6", link: `${base}/desenvolvimentomobile/aula6` },
      ],
    },
    {
      nome: "16. Segurança Digital",
      aulas: [
        { nome: "Aula 1", link: `${base}/segurancadigital/aula1` },
        { nome: "Aula 2", link: `${base}/segurancadigital/aula2` },
        { nome: "Aula 3", link: `${base}/segurancadigital/aula3` },
        { nome: "Aula 4", link: `${base}/segurancadigital/aula4` },
        { nome: "Aula 5", link: `${base}/segurancadigital/aula5` },
        { nome: "Aula 6", link: `${base}/segurancadigital/aula6` },
      ],
    },
    {
      nome: "17. Negócios Digitais e Comércio Eletrônico",
      aulas: [
        { nome: "Aula 1", link: `${base}/negociosdigitais/aula1` },
        { nome: "Aula 2", link: `${base}/negociosdigitais/aula2` },
        { nome: "Aula 3", link: `${base}/negociosdigitais/aula3` },
        { nome: "Aula 4", link: `${base}/negociosdigitais/aula4` },
        { nome: "Aula 5", link: `${base}/negociosdigitais/aula5` },
        { nome: "Aula 6", link: `${base}/negociosdigitais/aula6` },
      ],
    },
  ];

  let moduloAtivo = $state(null);

  function mostrarAulas(modulo) {
    if (moduloAtivo === modulo) {
      moduloAtivo = null;
    } else {
      moduloAtivo = modulo;
    }
  }

  function irParaInicio() {
    moduloAtivo = null;
  }
</script>

<aside transition:fly={{ x: -250, duration: 250 }}>
  <a id="inicio" href={base} onclick={irParaInicio}>Início</a>

  {#if modulos}
    {#each modulos as modulo}
      <button onclick={() => mostrarAulas(modulo.nome)}>{modulo.nome}</button>
      {#if moduloAtivo === modulo.nome && modulo.aulas.length > 0}
        <div transition:slide={{ duration: 250 }}>
          {#each modulo.aulas as aula}
            <a href={aula.link}>{aula.nome}</a>
          {/each}
        </div>
      {/if}
    {/each}
  {/if}
</aside>

<style>
  aside {
    height: 100vh;
    overflow-y: auto;
    overflow-x: hidden;
    scrollbar-width: none;
    background-color: #444;
    flex: 0 0 280px;
    display: flex;
    flex-direction: column;
    position: relative;
  }

  aside #inicio,
  aside button {
    flex-shrink: 0;
    background-color: transparent;
    width: 100%;
    padding: 0.8em 0.5em;
    font-size: 1em;
    text-decoration: none;
    text-align: start;
    color: #fff;
    transition: all 0.3s ease;
    text-transform: capitalize;
    font-weight: bold;
    border: none;
    cursor: pointer;
  }

  aside #inicio:hover,
  aside button:hover,
  aside div a:hover {
    background-color: #fff;
    color: #444;
  }

  aside div {
    flex-shrink: 0;
    width: 100%;
    display: flex;
    flex-direction: column;
  }

  aside div a {
    padding: 0.5em 1em;
    text-decoration: none;
    color: #ccc;
    transition: all 0.3s ease;
    display: block;
  }

  @media (max-width: 700px) {
    aside {
      position: fixed;
      top: 0;
      left: 0;
      width: 285px;
      z-index: 999;
      flex: none;
      box-shadow: 2px 0 10px 2px rgba(0, 0, 0, 0.3);
    }
  }
</style>
