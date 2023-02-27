<script>
  export default {
    data() {
      return {
        showMenu: false,
      };
    },
  };
</script>

<template>
    <div class="px-10 py-2 ">
      <div class="bg-green-800 bg-opacity-80 rounded ">
        <nav class="container px-auto py-2 mx-auto md:flex md:justify-between md:items-center">
          <div class="flex items-center justify-between">
            <router-link to="/" class="text-xl font-bold text-white md:text-2xl hover:text-green-400">
                Début
            </router-link>
          </div>
  
  
          <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
          <ul :class="showMenu ? 'flex' : 'hidden'" class="flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0">
            <li class="text-sm font-bold text-white hover:text-green-400">
              Présentation
            </li>
            <li class="text-sm font-bold text-white hover:text-green-400">
              Compétences
            </li>
            <li class="text-sm font-bold text-white hover:text-green-400">
              Projets
            </li>
            <li class="text-sm font-bold text-white hover:text-green-400">
              bidule
            </li>
            <li class="text-sm font-bold text-white hover:text-green-400">
              Langue
            </li>
          </ul>
        </nav>
      </div>
    </div>
</template>

