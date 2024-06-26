<script>
  export let y;

  export let tabs = [
    { name: "Projects ", link: "/#projects" },
    { name: "About me", link: "/#about" },
    { name: "Blog", link: "/#blog" }, // target: "_blank"
    { name: "Contact me", link: "/#contactMe" },
  ];
</script>

<!-- <header
  class=" sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between py-6"
> -->

<header
  class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid sm:hidden" +
    (y > 0
      ? " py-4 bg-slate-950 border-violet-450 text-white"
      : " py-6 bg-transparent border-transparent")}
>
  <h1 class="font-medium" on:click={() => window.scrollTo(0, 0)}>
    <b class="font-bold ubuntu cursor-pointer">Tanvi</b> <span class="">Sontakke</span>
  </h1>
  <div class="sm:flex ml-auto pr-4 items-center gap-4 hidden">
    {#each tabs as tab, index}
      <a href={tab.link} class="duration-200 hover:text-violet-500">
        <p>{tab.name}</p>
      </a>
    {/each}
    <!-- <a href="#" onclick="navToSection('projects')" class="duration-200 hover:text-violet-500">Projects</a>
    <a href="#" onclick="navToSection('about')" class="duration-200 hover:text-violet-500">About Me</a>
    <a href="#" onclick="navToSection('contact')" class="duration-200 hover:text-violet-500">Contact Me</a> -->
  </div>
</header>

<!--target={index === 2 ? "_blank" : ""}-->

<style>
  * {
    font-size: large;
  }

  body {
    margin: 0;
    padding: 0;
    font-size: 1rem;
  }

  header,
  main {
    width: 100%;
  }

  header {
    background-color: transition all 0.2s ease-in-out;
  }

  header.scrolled {
    background-color: #f5f5f5;
  }
</style>
