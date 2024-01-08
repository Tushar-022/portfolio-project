<section class="relative z-0 h-screen bg-black">
  <img
    src="/contact_bg.jpg"
    alt="bg"
    class="absolute top-0 left-0 w-full h-full object-cover opacity-30 mobile:opacity-50 -z-[1]"
  />

  <div class="flex flex-col h-full items-center justify-evenly text-white">
    <div class="text-center flex flex-col gap-y-4 mobile:gap-y-10">
      <h1 class="text-7xl font-bold font-sans">Let's Connect</h1>
      <p class="text-opacity-80 text-white font-light">
        Want to discuss the next big thing? Hire me? or develop a project with
        me?
        <br />
        I'm just a link away
      </p>
    </div>
    <img src="/screens/laptop/trustpoint/6.jpeg" alt="Trustpoint Screenshot" style="width: 20%; height: auto;">

    <div class="flex gap-4">
      <button
        class="bg-blue-500 text-white px-8 py-3 text-lg rounded-full shadow-md hover:bg-blue-700 transition duration-300"
        on:click={() => {
          window.open("https://www.linkedin.com/in/tushar-khandelwal-58522722b/");
        }}
        data-blobity-tooltip="Contact via Linkedin"
      >
        Connect on LinkedIn
      </button>
      <button
        class="bg-green-500 text-white px-8 py-3 text-lg rounded-full shadow-md hover:bg-green-700 transition duration-300"
        on:click={() => {
          window.open("https://github.com/Tushar-022");
        }}
        data-blobity-tooltip="View GitHub Profile"
      >
        GitHub Profile
      </button>
      <button
      class="bg-orange-500 text-white px-8 py-3 text-lg rounded-full shadow-md hover:bg-orange-700 transition duration-300"
      on:click={() => {
        window.open("https://leetcode.com/tushar05NITJ/");
      }}
      data-blobity-tooltip="View Leetcode Profile"
    >
      Leetcode Profile
    </button>
    </div>
  </div>
</section>
