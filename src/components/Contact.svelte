<section class="relative z-0 h-screen bg-black">
    <img
    src="/contact_bg.jpg"
    alt="bg"
    class="absolute top-0 left-0 w-full h-full object-cover opacity-30 md:opacity-50 z-[-2]"
  />
  
  
    <div class="flex flex-col h-full items-center justify-evenly text-white">
      <div class="text-center flex flex-col gap-y-4 md:gap-y-10">
        <h1 class="text-5xl font-bold font-sans m-2">Let's Connect</h1>
        <div class="flex items-start">
          <p class="text-opacity-80 text-2xl font-light mb-3">
            Tushar Khandelwal
            <br />
            I'm a sophomore at Nit Jalandhar pursuing BTech in Information Technology(2025).
            <br/>
            I have expertise in Data Structures and Algorithms and web development (MERN stack).
          </p>
        </div>
        <p>
          Want to discuss the next big thing? Hire me? or develop a project with me?
          <br />
          I'm just a click away
        </p>
      </div>
  
      <div class="flex flex-col mt-4 items-center">
        <img src="/screens/laptop/trustpoint/6.jpeg" alt="Trustpoint Screenshot" style="width: 20%; height: auto;">
  
        <div class="flex gap-x-7 m-10">
          <button class="bg-blue-500 text-white px-8 py-3 text-lg rounded-full shadow-md hover:bg-blue-700 transition duration-300"
            on:click={() => {
              window.open("https://www.linkedin.com/in/tushar-khandelwal-58522722b/");
            }}
            data-blobity-tooltip="Contact via Linkedin"
          >
            Connect on LinkedIn
          </button>
          <button class="bg-green-500 text-white px-8 py-3 text-lg rounded-full shadow-md hover:bg-green-700 transition duration-300"
            on:click={() => {
              window.open("https://github.com/Tushar-022");
            }}
            data-blobity-tooltip="View GitHub Profile"
          >
            GitHub Profile
          </button>
          <button class="bg-orange-500 text-white px-8 py-3 text-lg rounded-full shadow-md hover:bg-orange-700 transition duration-300"
            on:click={() => {
              window.open("https://leetcode.com/");
            }}
            data-blobity-tooltip="Leetcode Profile"
          >
            Leetcode Profile
          </button>
          <button class="bg-gray-500 text-white px-8 py-3 text-lg rounded-full shadow-md hover:bg-gray-700 transition duration-300"
            on:click={() => {
              window.open("https://drive.google.com/file/d/1tD4u3Z6BLXWS9aNC-Bvgs3GJKO3Zzknl/view?usp=sharing");
            }}
            data-blobity-tooltip="View Resume"
          >
            My Resume
          </button>
        </div>
      </div>
    </div>
  </section>
  