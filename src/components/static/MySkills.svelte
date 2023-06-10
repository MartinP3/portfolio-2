<script>
  import { Tooltip } from 'flowbite-svelte';
</script>

<section class="flex flex-col justify-center items-center">
  <h2 class="font-bold text-4xl text-center mb-4">My skills</h2>
  <div>
    <div>
      <h3 class="font-bold text-2xl">Languages & Frameworks</h3>
      <div class="grid grid-cols-4 md:flex gap-3 my-4">
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/HTML.svg" alt="HTML">
          <Tooltip>HTML</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/CSS.svg" alt="CSS">
          <Tooltip>CSS</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/JavaScript.svg" alt="Javascript">
          <Tooltip>JavaScript</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/React-Dark.svg" alt="React">
          <Tooltip>React</Tooltip>
        </div>
      </div>
      <h3 class="font-bold text-2xl">Tools & Libraries</h3>
      <div class="grid grid-cols-4 md:flex gap-3 my-4">
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Git.svg" alt="Git">
          <Tooltip>Git</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Github-Dark.svg" alt="GitHub">
          <Tooltip>GitHub</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Figma-Dark.svg" alt="Figma">
          <Tooltip>Figma</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/VSCode-Dark.svg" alt="Visual Studio Code">
          <Tooltip>Visual Studio Code</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Sass.svg" alt="Sass">
          <Tooltip>Sass</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Bootstrap.svg" alt="Bootstrap">
          <Tooltip>Bootstrap</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/TailwindCSS-Dark.svg" 
          alt="TailwindCSS">
          <Tooltip>TailwindCSS</Tooltip>
        </div>
        <div>
          <img class="icon" src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/StyledComponents.svg" alt="Styled Components">
          <Tooltip>Styled Components</Tooltip>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
::selection {
  background-color: #1d1d1d;
  color: #de6431;
  }

section {
  min-height: 40vh;
}

.icon {
  width: 4rem;
}

h2, h3 {
  font-family: "Poppins", sans-serif;
}
</style>