<script>
  import { Card } from "flowbite-svelte";
  import Image from "../assets/230602110916.png"

  let isFlipped = false;

  function toggleFlip() {
    isFlipped = !isFlipped;
  }
</script>

<section class="portfolioSection flex flex-col items-center my-4 gap-4">
  <div>
    <div class="flip-card w-96" class:flipped={isFlipped} on:click={toggleFlip} on:keydown={toggleFlip}>
      <div class="flip-card-inner">
        <div class="frontside">
          <Card padding="none" class="p-4">
            <img src={Image} alt="lol" />
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Semester Project 2</h5>
            <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
              Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
            </p>
          </Card>
        </div>
        <div class="backside">
          <Card padding="none" class="p-4 backside">
            <img src={Image} alt="lol" />
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">FLIPPED</h5>
            <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quam adipisci eius nesciunt reprehenderit. Eius ipsam
              excepturi asperiores quibusdam exercitationem amet numquam, accusantium, nihil, officiis dicta possimus nemo
              dolores aut facere.
            </p>
            <p class="text-center">Links here</p>
          </Card>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
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
</style>