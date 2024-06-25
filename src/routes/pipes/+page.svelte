<script>
  import image from "$lib/pipes.png"
</script>

<div class="py-6 px-4 flex font-style">
  <div>
    <p>
      Built a game similar to Flappy Bird in Python using PyGame, with a twist
      of our own, using a fish as the character.
    </p>
  </div>
  <!-- <img src="src\images\pipes.png" alt="fourth floor model" /> -->
  <img src={image} alt="fish bouncing thru pipes" />
</div>

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
