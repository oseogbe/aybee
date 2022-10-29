<template>
  <div class="relative h-screen bg-[url('@/assets/img/aybee-adayi.jpg')] bg-cover bg-no-repeat grayscale">
    <slot />
    <div class="h-screen absolute px-24">
      <div class="line h-2/6 w-0.5 ml-6 my-6 bg-white"></div>
      <div class="flex flex-col gap-y-6 ml-3">
        <font-awesome-icon font-size="24" color="#fff" :icon="['fab', 'facebook']"/>
        <font-awesome-icon font-size="24" color="#fff" :icon="['fab', 'twitter']"/>
        <font-awesome-icon font-size="24" color="#fff" :icon="['fab', 'instagram']"/>
      </div>
      <div class="line h-2/6 w-0.5 ml-6 mt-6 bg-white"></div>
    </div>
    <div class="w-100 absolute top-2/4 left-1/4 -translate-x-2/4 -translate-y-1/4 px-24">
      <h1 class="text-white text-8xl font-bold mb-6"><span class="px-4 py-1" style="background-color: #70707080;">Aybee Adayi</span></h1>
          <vue-typed-js
            :strings="['Creative Artist', 'Photographer', 'Videographer', 'Graphics Designer']"
            :loop="true"
            :smartBackspace='true'
            :typeSpeed='120'
            :backSpeed='50'
            :backDelay='70'
          >
            <p class="text-black text-5xl font-medium pl-4"><span class="typing"></span></p>
          </vue-typed-js>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Hero'

}
</script>
<style lang="scss" scoped>

</style>
