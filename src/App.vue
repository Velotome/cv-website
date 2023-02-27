<script setup>
  import Navbar from './components/Navbar.vue'
  import ContentBox from './components/ContentBox.vue'
</script>

<template>
  <div>
    <div  
    class="bg-[url('src/assets/landing.png')] w-full h-full bg-cover bg-no-repeat bg-fixed"
    style="min-height: 100vh;">
      <Navbar/>

      <!--Transparent rectangle landing-->
      <div 
      class="bg-transparent"
      style="min-height: 80vh;">
      </div>

      <!--Parallax content box-->
      <div>
        <ContentBox/>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
