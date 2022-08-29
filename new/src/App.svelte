<script>
  import { slide } from "svelte/transition"
  let showMenu = false
</script>

<section class="bg-yellow-400 h-screen flex flex-col">
  <div class="max-w-2xl w-full mx-auto relative z-50 h-1/3">
    <div class="flex justify-between items-start p-4">
      <div>
        <h1 class="{showMenu ? 'text-xl leading-none' : 'text-6xl'} font-black">
          the<br />bored<br />brothers
        </h1>
        <span class="mt-2 block text-xs"
          >© tbb, all rights reserved.<br />Not a member of the Cheezburger©
          Group.</span
        >
      </div>
      <button>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="2.5"
          stroke="currentColor"
          class="w-8 h-8"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M3.75 9h16.5m-16.5 6.75h16.5"
          />
        </svg>
      </button>
    </div>
  </div>

  <div
    class="max-w-2xl w-full mx-auto relative flex items-center z-50 h-1/3 p-4"
  >
    <h1 class="text-6xl font-bold text-left leading-tight">
      making boring stuff<br />for boring people<br />since 2022.
    </h1>
  </div>

  <footer
    class="max-w-2xl mx-auto px-4 flex items-end w-full justify-between h-1/3"
  >
    <span>Privacy Policy</span>
    <span>Twitter</span>
    <span>Terms of Service</span>
  </footer>

  <div class="max-w-2xl mx-auto p-4 flex-1 flex items-center h-1/3" />
  {#if showMenu}
    <div
      class="bg-white max-w-2xl mx-auto h-auto w-full absolute rounded-b-xl shadow-xl px-4 pt-36"
      transition:slide
    >
      <ul class="text-5xl font-bold divide-y">
        <li class="py-6">a day in the life</li>
        <li class="py-6">videogame logo quiz</li>
      </ul>
    </div>
  {/if}
</section>
