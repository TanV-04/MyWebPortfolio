<script>
  import image from "$lib/ngo.png"
</script>

<main class="flex flex-col flex-1 p-4">
  <div class="py-6 px-4 flex flex-col lg:flex-row items-center font-style">
    <div class="lg:w-1/2 lg:ml-4">
      <p>
        Created a user-friendly dashboard in Netbeans, especially helpful for service learning students, to simplify NGO searching, registration and donation process.
      </p>
    </div>
    <!-- <img src="src\images\ngo.png" alt="fourth floor model" /> -->
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
    height: 300px;
    border-color: black;
    border-style: groove;
    border-width: 5px;
  }

  p {
    margin-top: 155px;
  }
</style>
