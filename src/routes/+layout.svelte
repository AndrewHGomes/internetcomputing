<script>
  import Aside from "$lib/components/Aside.svelte";
  import Main from "$lib/components/Main.svelte";

  let { children } = $props();

  let menuAberto = $state(false);
  let larguraTela = $state(0);

  let exibirAside = $derived(larguraTela > 700 ? true : menuAberto);
</script>

<svelte:window bind:innerWidth={larguraTela} />

{#if exibirAside}
  <Aside />
{/if}

<Main bind:menuAberto>
  {@render children()}
</Main>

<style>
  :global(*) {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: "Segoe UI", sans-serif;
  }

  :global(body) {
    height: 100vh;
    width: 100%;
    color: #333;
    display: flex;
  }
</style>
