<script>
  import MusicCard from '$lib/MusicCard.svelte';
</script>

<h1>About Me</h1>

<p>Artists I like: (hover and scroll!)</p>

<div class="music-row">
  <MusicCard
    cover="/images/music/ram.png"
    alt="ram"
    title="Daft Punk"
    song="Touch"
    link="https://music.youtube.com/playlist?list=OLAK5uy_kNhM2yaBTOVwrcZJepB1C9P3-n5_Sfy5c"
  />

  <MusicCard
    cover="/images/music/pingfan.jpg"
    alt="pingfan"
    title="Mao Buyi"
    song="Jie"
    link="https://music.youtube.com/playlist?list=OLAK5uy_lp-NiQGCmBO3QqknnA1THvS2tohzNg110"
  />

  <MusicCard
    cover="/images/music/transatlanticism.jpg"
    alt="transatlanticism"
    title="Death Cab For Cutie"
    song="Grapevine Fires"
    link="https://music.youtube.com/playlist?list=OLAK5uy_lvk5k9W7M5y5NUEMx3A1miZ8QsIJkwAIE"
  />

  <MusicCard
    cover="/images/music/theluckyones.jpg"
    alt="lucky"
    title="Pentatonix"
    song="Coffee in Bed"
    link="https://music.youtube.com/playlist?list=OLAK5uy_lVkTDizjDp9B_niLWyMV-tI56NffEuIvc"
  />

  <MusicCard
    cover="/images/music/htbahb.jpg"
    alt="htbahb"
    title="Glass Animals"
    song="Youth"
    link="https://music.youtube.com/playlist?list=OLAK5uy_lvfdZw_P9YqQVYHZfkMSdRAzS8WTXWxrE"
  />

  <MusicCard
    cover="/images/music/aja.jpg"
    alt="aja"
    title="Steely Dan"
    song="Deacon Blues"
    link="https://music.youtube.com/playlist?list=OLAK5uy_ns_zqCLjZ6CXF0cji36OJNwTjH1YRYO_4"
  />

  <MusicCard
    cover="/images/music/teenage.png"
    alt="teenage"
    title="SEVENTEEN"
    song="Pinwheel"
    link="https://music.youtube.com/playlist?list=OLAK5uy_n1ss_dZ7ANz8PzJWSDpYH5UBimBXwmdF4"
  />

  <MusicCard
    cover="/images/music/ineveningair.jpg"
    alt="evening"
    title="Future Islands"
    song="Long Flight"
    link="https://music.youtube.com/playlist?list=OLAK5uy_moE8nHK_OIJiFpAho6UsrMpaol8xciHn8"
  />

  <MusicCard
    cover="/images/music/tate.jpeg"
    alt="airborne"
    title="The Airborne Toxic Event"
    song="Sometime Around Midnight (Acoustic)"
    link="https://music.youtube.com/playlist?list=OLAK5uy_muerAxw308CZ_CY0ouD6xBGbQuxsYtk_E"
  />
</div>

<style>
  .music-row {
    display: flex;
    gap: 1rem;
    overflow-x: auto;
    margin-top: 1.5rem;
  }
</style>
