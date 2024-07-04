<script>
  import Step from "./Step.svelte";
  import image from "$lib/profileImg.jpg"
  import i from "$lib/letter.svg"

  let steps = [
    {
      name: "Global News in Marathi: Headlines & Insights",
      icon: "fa-solid fa-language text-purple-300",
      description:
        "Created a GUI for text extraction, summarization, and translation using NetBeans and Flask, to demonstrate the offline functionality of such applications in rural parts of India.",
      href: "/pbl1",
    },
    {
      name: "Dodge the Pipes: Marine Edition",
      icon: "fa-solid fa-gamepad text-purple-300",
      description:
        "Built a game similar to Flappy Bird in Python using PyGame, with a twist of our own, using a fish as the character.",
      href: "/pipes",
    },
    {
      name: "Engineering Graphics Simulator",
      icon: "fa-solid fa-compass-drafting text-purple-300",
      description:
        "Built a simulator for visualizing lines using angles and distances as input for our Engineering Graphics Lab in semester 1.",
      href: "/graphics",
    },
    {
      name: "NGOLogs: A Simplified NGO Engagement System",
      icon: "fa-solid fa-database text-purple-300",
      description:
        "Created a user-friendly dashboard in NetBeans for service learning students to easily search, register with, and donate to NGOs, streamlining the process significantly.",
      href: "/ngoLogs",
    },
    {
      name: "Virtual Replica of SIT's CS Department",
      icon: "fa-solid fa-vr-cardboard text-purple-300",
      description:
        "We created a virtual version of SIT's Computer Science Department with a team of three students, led by the department's HoD. This model was used to test custom VR goggles by another team and formed the basis for a 3D racing game as a part of an event at our TechFest '23.",
      href: "/fourthFloor",
    },
    {
      name: "Virtual Lab Designing for School-Children",
      icon: "fa-solid fa-school text-purple-300",
      description:
        "As a part of my internship in first year, me and my partner were responsible for designing virtual and interactive tech-labs for school-children and testing the models using an Occulus. ",
      href: "/guruji",
    },

    {
      name: "Personal Portfolio",
      icon: "fa-solid fa-briefcase text-purple-300",
      description:
        "Made my personal portfolio.",
      href: "/portfolio",
    },

    {
      name: "Recipe Website Template",
      icon: "fa-solid fa-bowl-food text-purple-300",
      description:
        "Developed a ready to use template/website for food bloggers.",
      href: "/recipeWebsite",
    },
  ];

  let benefits = [
    { name: "Team Work", description: "" },
    { name: "Effective Communication", description: "" },
    { name: "Project Management", description: "" },
  ];

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
    // {
    //   title: "How the World Frustrates Me",
    //   smallDesc:
    //     "Caught in a dystopian present, I wonder if my dreams for a better future are just a fantasy amidst political games and environmental crises.",
    //   href: "",
    // },
    {
      title: "College",
      smallDesc:
        "Up till now, college has been a whirlwing of growth and self-reflection, shaping me into someone who's learning to navigate expectations and make my own future.",
      href: "/college",
    },
  ];
</script>

<main class="flex flex-col flex-1 p-4">
  <section
    id="introPage"
    class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
  >
    <div
      class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
    >
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi! I'm <span class="ubuntu text-violet-900">Tanvi</span> Sontakke.<br
        />
        Student, <span class="ubuntu text-violet-600"> Coder</span>, Avid
        Learner
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        My <span class="text-violet-900">favorite tech </span>includes Java,
        C++, Svelte, and MySQL.
      </p>
    </div>

    <div class="relative shadow-2xl grid place-items-center">
      <!-- <img
        src="src\images\profileImg.jpg"
        alt="profile image"
        class="object-cover z-[2] max-h-[70vh]"
      /> -->
      <img
      src={image}
      alt="profile image"
      class="object-cover z-[2] max-h-[70vh]"
    />
    </div>
  </section>

  <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
      <h6 class="text-lg sm:text xl md:text-2xl">Projects</h6>

      <!-- <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        Want to see <span class="ubuntu text-violet-700">more of my work</span>?
      </h3> -->
    </div>

    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={steps[0]}>
        <p>
          Created using <strong class="text-violet-900">Java, Flask</strong>
        </p>
      </Step>
      <Step step={steps[1]}>
        <p>
          Created using <strong class="text-violet-900">Python.</strong>
        </p>
      </Step>
      <Step step={steps[2]}>
        <p>
          Created using <strong class="text-violet-900">Python.</strong>
        </p>
      </Step>

      <Step step={steps[3]}>
        <p>
          Created using <strong class="text-violet-900">Java, MySQL.</strong>
        </p>
      </Step>

      <Step step={steps[4]}>
        <p>
          Created using <strong class="text-violet-900">Blender, Unity.</strong>
        </p>
      </Step>

      <Step step={steps[5]}>
        <p>
          Created using <strong class="text-violet-900">Blender.</strong>
        </p>
      </Step>

      <Step step={steps[6]}>
        <p>
          Created using <strong class="text-violet-900">Svelte, HTML, CSS, JS.</strong>
        </p>
      </Step>

      <Step step={steps[7]}>
        <p>
          Created using <strong class="text-violet-900">Svelte, HTML, CSS, JS.</strong>
        </p>
      </Step>
    </div>
  </section>

  <section
    id="about"
    class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
  >
    <div
      class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
    >
      <h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        A bit <span class="ubuntu text-violet-900">about</span> me.
      </h3>
    </div>

    <p
      class="mx-auto ubuntu font-semibold text-lg sm:text-xl md:text-2xl text-center"
    >
      Hey there! I'm a Computer Science student at SIT, Pune, fueled by
      curiosity and enthusiasm about everything (quite literally!). I thrive on
      meeting new people and lending a helping hand while staying up-to-date
      with cutting-edge technology. However, outer space has always piqued my
      interest! <br /> Some of my strong points are:
    </p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
      {#each benefits as benefit, index}
        <div class="flex gap-6 sm:gap-8">
          <p
            class="ubuntu text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
          >
            0{index + 1}
          </p>
          <div class="flex flex-col gap-6 sm:gap-8">
            <h3 class="text-2xl sm:text-3xl md:text-5xl">
              {benefit.name}
            </h3>
            <p>{benefit.description}</p>
          </div>
        </div>
      {/each}
    </div>
  </section>

  <hr style="border-top: 2px solid purple;"/>

  <section id="blog" class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
      <h6 class="text-lg sm:text xl md:text-2xl" style="font-weight: bold;">My Blogs</h6>
    </div>
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
  </section>

  <section id="contactMe"></section>
</main>

<!-- <link rel="icon" type="image/svg+xml" href={i}/> -->

<style>
  .text-violet-900 {
    font-weight: bold;
  }

  .object-cover {
    border-radius: 90px;
  }

  .grid.grid-cols-1.lg:grid-cols-3 {
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
  }

  .fa-solid {
    color: #e3e0e8;
    font-size: 1rem;
  }

  .blog1 {
    margin-bottom: 0.2px;
  }

  a {
    font-weight: bold;
  }
</style>
