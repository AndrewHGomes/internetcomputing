<script>
  import { base } from "$app/paths";
  let { modulo, aulas } = $props();
</script>

<div class="audio-wrapper">
  {#each aulas as numero}
    <div class="item">
      <span>{numero}</span>
      <audio src="{base}/audios/audios{modulo}/aula{numero}.mp3" controls
      ></audio>
    </div>
  {/each}
</div>

<style>
  .audio-wrapper {
    display: flex;
    flex-direction: column;
    gap: 8px;
    margin: 1rem 0;
  }

  .item {
    display: flex;
    align-items: center;
    gap: 0.5em;
    background: rgba(0, 0, 170, 0.03);
    padding: 5px 10px;
    border-radius: 5px;
    border: 1px solid #ddd;
    box-shadow: 0 0 10px 2px rgba(0, 0, 0, 0.05);
  }

  .item span {
    font-size: 0.9rem;
    font-weight: bold;
    color: #aaa;
    font-family: sans-serif;
  }

  audio {
    flex: 1;
    height: 1.5rem;
  }

  audio::-webkit-media-controls-enclosure {
    background-color: rgba(0, 0, 0, 0);
  }
</style>
