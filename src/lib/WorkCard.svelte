<script>
  let { logo, alt, title, dates, location, children } = $props();
</script>

<div class="work-card">
  <div class="header">
    <div class="logo-box">
      <img src={logo} {alt} class="logo" />
    </div>
    <div class="when-where">
      <p>{dates}</p>
      <p>{location}</p>
    </div>
  </div>

  <p class="job-title">{title}</p>
  <div class="job-info">
    {@render children?.()}
  </div>
</div>

<style>
  .work-card {
    width: 100%;
    box-sizing: border-box;
    border: 1px solid var(--color-border);
    padding: 1.5rem;
  }

  .header {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
  }

  .logo-box {
    box-sizing: border-box;
    height: 72px;
    flex: 0 0 auto;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 1px solid var(--color-border);
    padding: 0.5rem;
    overflow: hidden;
  }

  .logo {
    height: 100%;
    width: auto;
    object-fit: contain;
    display: block;
  }

  .when-where {
    text-align: right;
  }

  .when-where p {
    margin: 0;
  }

  .job-title {
    margin: 1rem 0 0;
    text-align: left;
  }

  .job-info {
    margin-top: 0.25rem;
    text-align: left;
  }
</style>
