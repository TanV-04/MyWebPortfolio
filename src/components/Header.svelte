<script>
  export let y;

  export let tabs = [
    { name: "Projects ", link: "/#projects" },
    { name: "About me", link: "/#about" },
    { name: "Blog", link: "/#blog" }, // target: "_blank"
    { name: "Contact me", link: "/#contactMe" },
  ];

  let isMobileMenuOpen  = false;

  function toggleMobileMenu() {
    isMobileMenuOpen = !isMobileMenuOpen;
  }

</script>

<!-- <header
  class=" sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between py-6"
> -->

<header
  class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid" +
    (y > 0
      ? " py-4 bg-slate-950 border-violet-450 text-white"
      : " py-6 bg-transparent border-transparent")}>

  <!--logo and name-->

  <h1 class="font-medium" on:click={() => window.scrollTo(0, 0)}>
    <b class="font-bold ubuntu cursor-pointer">Tanvi</b> <span class="">Sontakke</span>
  </h1>

  <!--mobile menu toggle button-->

  <button type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="mobile-menu" aria-expanded={isMobileMenuOpen} on:click={toggleMobileMenu}>
    <span class="sr-only">Open main menu</span>
    <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
      <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
    </svg>
  </button>

  <div class={`absolute top-0 left-0 w-full bg-white shadow-lg md:hidden ${isMobileMenuOpen ? 'block' : 'hidden'}`} id="mobile-menu">
    <ul class="p-4">
      {#each tabs as tab}
        <li>
          <a href={tab.link} class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100">{tab.name}</a>
        </li>
      {/each}
    </ul>
  </div>

  <!--desktop menu-->

  <div class="sm:flex ml-auto pr-4 items-center gap-4 hidden">
    {#each tabs as tab, index}
      <a href={tab.link} class="duration-200 hover:text-violet-500 hidden sm:block">
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

  header {
    width: 100%;
  }

  header {
    background-color: transition all 0.2s ease-in-out;
  }

  header.scrolled {
    background-color: #f5f5f5;
  }

</style>
