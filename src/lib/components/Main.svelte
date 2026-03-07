<script>
  let { children, menuAberto = $bindable() } = $props();
</script>

<main>
  <button
    type="button"
    onclick={() => (menuAberto = !menuAberto)}
    class="btn-menu"
    aria-label="Abrir menu de navegação"
  >
    <i class="fa-solid {menuAberto ? 'fa-xmark' : 'fa-bars'}"></i>
  </button>

  {@render children()}
</main>

<style>
  main {
    flex: 1;
    height: 100vh;
    overflow-y: auto;
    overflow-x: hidden;
    padding: 1.5em 1em;
    line-height: 1.4;
    width: 100%;
  }

  main .btn-menu {
    display: none;
    position: fixed;
    top: 0.6em;
    right: 0.8em;
    background-color: #333;
    color: #fff;
    font-size: 1em;
    padding: 0.5em;
    border: none;
    border-radius: 3px;
    cursor: pointer;
    z-index: 1000;
  }

  :global(h1) {
    color: #a00;
    margin: 0.5em 0;
  }

  :global(h2) {
    color: #00a;
    margin: 0.5em 0;
  }

  :global(h3) {
    color: #f80;
    margin: 0.5em 0;
  }

  :global(h4) {
    color: #a00;
    margin: 0.5em 0;
  }

  :global(p) {
    margin: 0.5em 0;
    text-align: justify;
  }

  :global(strong) {
    color: #0a0;
  }

  :global(ul),
  :global(ol) {
    padding-left: 1em;
  }

  :global(li) {
    padding: 0.3em 0;
    text-align: justify;
  }

  @media (max-width: 700px) {
    main .btn-menu {
      display: block;
      box-shadow: 0 0 10px 4px rgba(0, 0, 0, 0.3);
    }

    :global(h1) {
      text-align: center;
    }
  }
</style>
