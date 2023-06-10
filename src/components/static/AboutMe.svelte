<script>
  import { P, Img } from "flowbite-svelte";
  import Image from "../../assets/230602110916.png"

  let isFlipped = false;

  function toggleFlip() {
    isFlipped = !isFlipped;
}
</script>
<section class="flex flex-col sm:flex-col items-center md:flex-row m-4 justify-center md:gap-14">
  <div class="flip-card w-80" class:flipped={isFlipped} on:click={toggleFlip} on:keyup={toggleFlip}>
    <div class="flip-card-inner mb-36 md:mb-0">
      <div class="frontside flex items-center">
        <P class="max-w-xl mb-4 md:mx-2">
          <h1 class="text-4xl font-bold mb-2 title">About me</h1>
          <p class="text-xl description">I am a 24 year old student from Norway that studied at Noroff's Frontend Development course.</p>
          <p class="text-xl description">
            In my freetime I enjoy reading fantasy, playing video games and relaxing with my friends.
          </p>
          <p class="text-center text-xl">1/2</p>
        </P>
      </div>
      <div class="backside flex items-center">
        <P class="max-w-xl mb-4 md:mx-2">
          <h1 class="text-4xl font-bold mb-2 title">My path</h1>
          <p class="text-xl description">I have been all over the place study wise and experienced a fair bit, from almost becoming a ship engineer, to almost becoming an economist only to finally find the path for me in webdev</p>
          <p class="text-center text-xl">2/2</p>
        </P>
      </div>
    </div>
  </div>
  <Img src={Image} alt="Picture of Martin Pedersen" size="max-w-[20rem]" class="filter grayscale"/>
</section>
<style>
  .title {
    font-family: 'Poppins', sans-serif;
  }
  .description {
    font-family: 'Montserrat', sans-serif;
  }

  .flip-card {
    perspective: 900px;
    cursor: pointer;
  }

  .flip-card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    transform-style: preserve-3d;
    transition: transform 0.5s;
  }

  .flip-card.flipped .flip-card-inner {
    transform: rotateY(180deg);
  }

  .frontside,
  .backside {
    position: absolute;
    width: 100%;
    height: 100%;
    backface-visibility: hidden;
  }

  .backside {
    transform: rotateY(180deg);
  }
  
 ::selection {
  background-color: #1d1d1d;
  color: #de6431;
}
</style>