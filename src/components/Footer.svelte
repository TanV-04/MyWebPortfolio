<script>
  import pdf from "$lib/tanvi_sontakke_resume1.pdf";
</script>

<footer
  class="py-20 sm:py-32 bg:black border-t border-solid border-violet-950 flex flex-col gap-4 sm:Gap-8 justify-center items-center"
>
  <p class="px-4 py-2 bg-white text-slate-950 font-medium connect-me">
    Connect with me &darr;
  </p>
  <div class="flex flex-col gap-4 items-center justify-center">
    <p><b class="pr-2">Email</b> aretanvi@gmail.com</p>
    <p>
      <b class="pr-2">Github</b>
      <a
        href="https://github.com/TanV-04"
        class="text-violet-900"
        target="_blank"
      >
        TanV<sup
          ><span class="text-xs scale-75pl-0.5">
            <i
              class="fa-solid fa-arrow-up-right-from-square text-xs scale-[75%]"
            />
          </span></sup
        >
      </a>
    </p>

    <p>
      <b class="pr-2">LinkedIn</b>
      <a
        href="https://www.linkedin.com/in/tanvi-sontakke-298407279/"
        class="text-violet-900"
        target="_blank"
      >
        Tanvi Sontakke<sup
          ><span class="text-xs scale-75pl-0.5">
            <i
              class="fa-solid fa-arrow-up-right-from-square text-xs scale-[75%]"
            />
          </span></sup
        >
      </a>
    </p>

    <!-- <a href="src/files/tanvi_sontakke_resume.pdf" style="font-weight: bold;">Resume</a> in dev mode -->
    <a href={pdf} style="font-weight: bold;">Resume</a>
  </div>
</footer>

<style>
  div {
    font-size: large;
    font-weight: bold;
  }

  .connect-me {
    border-radius: 10px;
    font-weight: bold;
  }
</style>
