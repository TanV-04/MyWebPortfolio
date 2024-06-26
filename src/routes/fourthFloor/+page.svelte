<script>
  import image from "$lib/fourthFloor.png";
</script>

<main class="flex flex-col flex-1 p-4">
  <div class="py-6 px-4 flex flex-col lg:flex-row items-center font-style">
    <div class="lg:w-1/2 lg:ml-4">
      <p>
        Created 3D models for recreating the Computer Science Department using
        Blender and Unity for website integration, enhancing campus accessibility
        for remote students. The model can be made into a VR application for a
        better experience.
      </p>
    </div>
    <!-- <img src="src\images\fourthFloor.png" alt="fourth floor model"/> in dev mode-->
    <img class="lg:mr-4 mb-4 lg:mb-0 rounded-lg border-4 border-black lg:w-1/2" src={image} alt="fourth floor model" />
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
    height: 400px;
    border-color: black;
    border-style: groove;
    border-width: 5px;
  }

  p {
    margin-top: 155px;
  }
</style>
