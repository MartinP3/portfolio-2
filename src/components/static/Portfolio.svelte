<script>
  import { Card } from "flowbite-svelte";
  import Image from "../../assets/230602110916.png"
</script>

<section class="flex flex-col justify-center items-center mb-4 mt-8">
  <h1 class="text-4xl font-bold title mb-4">My projects</h1>
  <div class="grid grid-cols-1 lg:grid-cols-3 gap-4">
    <Card padding="none" class="p-4">
      <img src={Image} alt="front page of semester project 2 site" />
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Semester Project 2</h5>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
        In the Semester Project 2 I made a website for auctions, where you could bid on items and sell your own items.
      </p>
      <div class="flex justify-center gap-2">
        <a href="https://github.com" target="_blank" class="projectLinks"><i class="fa-brands fa-github"></i>GitHub</a>
        <a href="https://github.com" target="_blank" class="projectLinks"><i class="fa-solid fa-paper-plane"></i>Site</a>
      </div>
    </Card>
    <Card padding="none" class="p-4">
      <img src={Image} alt="front page of Javascript Frameworks site" />
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Javascript Frameworks</h5>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
        In the JavaScript frameworks course I made a online shopping website where users could add items to their cart and purchase them.
      </p>
      <div class="flex justify-center gap-2">
        <a href="https://github.com" target="_blank" class="projectLinks"><i class="fa-brands fa-github"></i>GitHub</a>
        <a href="https://github.com" target="_blank" class="projectLinks"><i class="fa-solid fa-paper-plane"></i>Site</a>
      </div>
    </Card>
    <Card padding="none" class="p-4">
      <img src={Image} alt="front page of project exam 2 site" />
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Project Exam 2</h5>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
        In the project exam 2 course I made a website for a fictional company where users could rent out locations and book locations that others listed.
      </p>
      <div class="flex justify-center gap-2">
        <a href="https://github.com" target="_blank" class="projectLinks"><i class="fa-brands fa-github"></i>GitHub</a>
        <a href="https://github.com" target="_blank" class="projectLinks"><i class="fa-solid fa-paper-plane"></i>Site</a>
      </div>
    </Card>
  </div>
</section>

<style>
  .title, h5 {
    font-family: 'Poppins', sans-serif;
  }

  p {
    font-family: "Montserrat", sans-serif;
  }

  section {
    min-height: 70vh;
  }

  .projectLinks {
    color: #6b7280;
    transition: color 0.1s ease;
  }

  .projectLinks:hover {
    color: #de6431;
  }

  ::selection {
  background-color: #1d1d1d;
  color: #de6431;
  }
</style>