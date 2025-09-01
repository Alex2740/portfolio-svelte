<script>
  let activeTab = 'about'; // Initialize with the default active tab
</script>

<div class="flex h-screen max-w-6xl mx-auto gap-4 p-4">
  <div class="bg-pink-500 rounded-2xl w-3xs flex-none">
    <div>
      <div></div>
      <h1>Valentin Plantard-Wahl</h1>
      <span>Developper</span>
    </div>
    <hr />
    <div>
      mail
      phone
      birthday
      location
    </div>
    <div>
      github
    </div>
  </div>
  <div class="bg-purple-500 rounded-2xl grow relative overflow-ellipsis">
    <nav class="bg-blue-400 rounded-2xl float-right">
      <button on:click={() => activeTab = 'about'}>About</button>
      <button on:click={() => activeTab = 'resume'}>Resume</button>
      <button on:click={() => activeTab = 'portfolio'}>Portfolio</button>
      <button on:click={() => activeTab = 'contact'}>Contact</button>
    </nav>
    <main>
      {#if activeTab === 'about'}
        <h2>About me</h2>
        <p class="text-pretty">Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore, aut ab nam sint culpa dolorum eaque natus accusamus vero placeat nostrum fugiat vel, aliquid obcaecati! Quidem veniam nisi consequatur sint.</p>
        <h3>What I'm doing</h3>
        <div>grid</div>
        <h3>Testimonials</h3>
        <div>carrousel testi</div>
        <h3>Clients</h3>
        <div>carrousel client</div>
      {:else if activeTab === 'resume'}
        <h2>Resume</h2>
        <div>Education</div>
        <div>Experience</div>
        <div>Skill</div>
        <div>loader for skill</div>
      {:else if activeTab === 'portfolio'}
        <h2>Portfolio</h2>
        <div>Selector</div>
        <div>Grid project</div>
      {:else if activeTab === 'contact'}
        <h2>Contact</h2>
        <div>map</div>
        <h3>Contact form</h3>
        <div>contact form</div>
      {/if}
    </main>
  </div>
</div>

<style>
  :root {
    --main-width: calc();
  }
</style>
