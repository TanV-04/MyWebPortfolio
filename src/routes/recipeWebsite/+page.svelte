<script>
  import image from "$lib/recipe.png";
</script>

<main class="flex flex-col flex-1 p-4">
  <div class="py-6 px-10 flex flex-col lg:flex-row items-center font-style">
    <div class="lg:w-1/2 lg:ml-4">
      <p>Developed a ready to use template/website for food bloggers.</p>
    </div>
    <!-- <img src="src\images\guruji.png" alt="fourth floor model" /> -->
    <img
      src={image}
      class="lg:mr-4 mb-4 lg:mb-0 rounded-lg border-4 border-black lg:w-1/2"
      alt="fourth floor model"
    />
  </div>
</main>

<style>
  .font-style {
    font-weight: bold;
    font-size: larger;
    float: left;
    width: 100%;
  }

  img {
    margin-top: 15px;
    float: right;
    border-radius: 10px;
    width: 500px;
    height: 300px;
    border-color: black;
    border-style: groove;
    border-width: 5px;
  }

  p {
    margin-top: 155px;
  }
</style>
