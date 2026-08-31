<script>
  import '../app.css';
  let { children } = $props();
</script>

<svelte:head>
  <title>daniel miao</title>
</svelte:head>

<div class="page-wrapper">
  <div class="page">
    <div class="sidebar">
      <div class="profile">
        <img class="profile-pic" src="/images/miaomiaogato.png" alt="Miaomiaogato" />
        <div class="identity">
          <p class="name">daniel miao</p>
          <p class="pronouns">he/him</p>
        </div>
      </div>
      <div class="nav-links">
        <a href="/">Home</a>
        <a href="/news">News</a>
        <a href="/about">About Me</a>
        <a href="/projects">Projects</a>
        <a href="/blog">Blog</a>
        <a href="/contact">Contact</a>
      </div>
    </div>
    <div class="content">
      {@render children()}
    </div>
  </div>
</div>

<style>
  .page-wrapper {
    height: 100vh;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .page {
    --sidebar-width: 200px;
    display: flex;
    width: 100%;
    max-width: 1200px;
    height: 70vh;
    /* margin-left: calc(var(--sidebar-width) / -1.5); */
  }

  .sidebar {
    --pfp-width: 180px;
    flex: 0 0 var(--sidebar-width);
    padding: 1rem;
    overflow-y: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 2rem;
  }

  .profile {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1.5rem;
  }

  .profile-pic {
    width: var(--pfp-width);
    height: var(--pfp-width);
    border-radius: 50%;
    object-fit: cover;
  }

  .identity {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.25rem;
  }

  .name,
  .pronouns {
    margin: 0;
    color: var(--color-black);
    text-align: center;
  }

  .nav-links {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
    width: calc(var(--pfp-width) / 2);
  }

  .nav-links a {
    color: var(--color-gray);
    text-decoration: none;
  }

  .nav-links a:hover {
    color: var(--color-black);
  }

  .content {
    flex: 1;
    background-color: var(--color-white);
    border: 1px solid var(--color-border);
    padding: 2.5rem;
    overflow-y: auto;
  }
</style>