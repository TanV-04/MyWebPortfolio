<script>
  import "../app.css";
  import Footer from "../components/Footer.svelte";
  import Header from "../components/Header.svelte";

  let y;
  let innerWidth = 0;
  let showScrollButton = false;
  let innerHeight = 0;

  function goTop() {
    document.body.scrollIntoView();
  }

  $: showScrollButton = y > 100;
</script>

<div
  class="container relative flex flex-col max-w-[1400px] mx-auto w-full text-sm sm:text-base min-h-screen"
>
  <div class="fixed bottom-6 right-6 z-50" style="{showScrollButton ? 'opacity: 1; pointer-events: auto;' : 'opacity: 0; pointer-events: none;'}">
    <button
      on:click={goTop}
      class="ml-auto rounded-full aspect-square bg-slate-900 text-violet-400 px-3 sm:px-4 hover:bg-slate-800 cursor-pointer aspect-square grid place-items-center"
    >
      <i class="fa-solid fa-arrow-up" />
    </button>
  </div>
  <Header {y} {innerHeight} />
  <slot />
  <Footer />
</div>
<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth />
