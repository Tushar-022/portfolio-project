<script>
  import FluidSim from "./FluidSim.svelte";

  import { onDestroy, onMount } from "svelte";
  let observer, sect;
  let entry = { isIntersecting: false };
  let flash = false;

  onMount(() => {
    observer = new IntersectionObserver(
      ([e]) => {
        entry = e;
      },
      {
        threshold: 0.69,
      }
    );
    observer.observe(sect);
  });

  onDestroy(() => {
    observer.disconnect();
  });
</script>

<section
  bind:this={sect}
  class="about bg-black observed relative overflow-hidden mobile:pointer-events-none"
>
  {#if entry.isIntersecting}
    <FluidSim />
  {/if}

  <div
    class="relative text-primary py-16 z-[1] mix-blend-difference pointer-events-none flex flex-col items-center justify-center text-center"
  >
    <div class="font-bold text-4xl mobile:text-3xl">Get to know me</div>
    <div class="font-black text-7xl py-8 mobile:text-4xl">
      Tushar Khandelwal
    </div>
    <div
      class="py-12 font-semibold text-2xl p-page text-justify mobile:py-3 mobile:text-lg"
    >
    Hello! I am a highly driven and passionate Final Year Undergrad at  Nit Jalandhar ,majoring in Information & Technology Branch, with a strong interest in Algorithmic Problem Solving, Data Structures, and Algorithms. I have achieved remarkable success in Programming, climbing up to the top 0.01%  Programmers in India, and securing a rank under 100 on HackWithInfy, the hackathon by Infosys across the country.

I am proud to have ranked in the top 65 teams during Amazon Hackon 2024, a competition involving prestigious institutions including IITs and NITs. This achievement showcases my hard work, dedication, and passion for problem-solving.

With my strong problem-solving skills, dedication, and passion, I am confident that I can contribute significantly to any organization I work with. I am eager to take on new challenges and learn from the best in the industry.

Thank you for taking the time to read about me, and I look forward to connecting with you!
    </div>
  </div>

  <div
    class="absolute h-2/6 top-0 w-full pointer-events-none"
    style="background-image: linear-gradient(to bottom, rgb(var(--background)), transparent);"
  />
  <div
    class="absolute h-2/6 bottom-0 w-full pointer-events-none"
    style="background-image: linear-gradient(to top, rgb(var(--background)), transparent);"
  />
</section>
