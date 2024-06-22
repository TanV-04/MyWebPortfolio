<script>
  let blogs = [
    {
      title: "My First Blog",
      smallDesc: "Click here to read my first ever blog!",
      href: "/firstBlog",
    },
    {
      title: "Metaverse",
      smallDesc:
        "The metaverse combines AI, virtual environments, and immersive tech to revolutionize how we interact online, shaping the future of the Internet. Click to find out more!",
      href: "/metaverse",
    },
    {
      title: "2020",
      href: "/covid",
      smallDesc:
        "The COVID-19 pandemic completely transformed our daily lives, confronting us with a new reality looming over the horizon yet humans persevered with resilience and courage.",
    },
    {
      title: "Indian Parents and Education",
      smallDesc:
        "To pursue our passions or bow to societal expectations: the age-old struggle between staying true to ourselves and seeking approval, where happiness outweighs riches.",
      href: "/indianEd",
    },
    {
      title: "Pollution",
      smallDesc:
        "The global climate crisis is ignored like a plastic bag flying past, but its impact on children, health, and wildlife demands urgent action beyond excuses and political games.",
      href: "/pollution",
    },
    {
      title: "LLMs and Green Coding",
      smallDesc:
        "Training Large Language Models like ChatGPT emits carbon like a speeding car around the Earth's equator 300 times, but green coding offers hope for a greener tech future.",
      href: "/llms",
    },
    {
      title: "How the World Frustrates Me",
      smallDesc:
        "Caught in a dystopian present, I wonder if my dreams for a better future are just a fantasy amidst political games and environmental crises.",
      href: "",
    },
    {
      title: "College",
      smallDesc:
        "Up till now, college has been a whirlwing of growth and self-reflection, shaping me into someone who's learning to navigate expectations and make my own future.",
      href: "/college",
    },
  ];
</script>

<!-- <button class="btn btn-primary py-10" on:click={() => (window.location.href = "/")}>
  Back to home
</button> -->


{#each blogs as blog}
  <a href={blog.href}>
    <div class="outer-container">
      <div
        class="blog1 p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center group cursor-pointer hover:border-violet-400 duration-200"
      >
        <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">
          {blog.title}
        </h3>
        <p class="text-indigo-900 mt-4">{blog.smallDesc}</p>
        <div class="flex-1 flex justify-between gap-4 items-center">
          <div
            class="ml-auto cursor-pointer hover:text-slate-900 duration-200 relative after:absolute after:top-0 after:h-0 after:right-full after:bg-white after:w-full after:h-full after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden"
          >
            <p class="relative z-4">Go to &rarr;</p>
          </div>
        </div>
      </div>
    </div>
  </a>
{/each}


<style>
  .blog1 {
    margin-bottom: 140px;
  }

  a {
    font-weight: bold;
  }
</style>
