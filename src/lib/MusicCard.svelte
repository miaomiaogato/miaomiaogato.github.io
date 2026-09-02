<script>
  let { cover, alt, song, title, link } = $props();
</script>

<div class="music-card-wrapper">
  <a class="music-card" href={link} target="_blank" rel="noopener noreferrer">
    <img src={cover} {alt} class="cover" />
    <div class="overlay">
      <p>Favorite Song: {song}</p>
    </div>
  </a>
  <p style="text-align: center;">{title}</p>
</div>

<style>
  .music-card-wrapper {
    --card-size: 200px;
    width: var(--card-size);
    flex: 0 0 var(--card-size);
  }

  .music-card {
    display: block;
    position: relative;
    box-sizing: border-box;
    width: var(--card-size);
    height: var(--card-size);
    border: 1px solid var(--color-border);
    padding: 0.75rem;
    overflow: hidden;
  }

  .cover {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }

  .overlay {
    position: absolute;
    inset: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 0.75rem;
    background-color: var(--color-overlay);
    color: var(--color-white);
    opacity: 0;
    transition: opacity var(--ease-overlay) ease;
    pointer-events: none;
  }

  .music-card:hover .overlay {
    opacity: 1;
  }

  .overlay p {
    margin: 0;
  }
</style>
