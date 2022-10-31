<template>
  <div id="hero" class="relative h-screen bg-[url('@/assets/img/aybee-adayi.jpg')] bg-cover bg-center bg-no-repeat grayscale">
    <slot />
    <div class="h-screen absolute px-2 md:px-8">
      <div class="h-3/6 md:h-2/6 w-0.5 ml-6 my-6 bg-transparent md:bg-black"></div>
      <div class="hidden md:flex flex-col gap-y-6 ml-3">
        <a href="https://web.facebook.com/abraham.abel.752/" target="_blank">
          <font-awesome-icon font-size="24" color="#000" :icon="['fab', 'facebook']"/>
        </a>
        <a style="margin-left: 2px;" href="https://instagram.com/aybee_adayi/" target="_blank">
          <font-awesome-icon font-size="24" color="#000" :icon="['fab', 'instagram']"/>
        </a>
        <a href="https://www.youtube.com/channel/UC4bO-Zg_yqPOdyKU_K2ZBVA/" target="_blank">
          <font-awesome-icon font-size="24" color="#000" :icon="['fab', 'youtube']"/>
        </a>
      </div>
      <div class="flex flex-col md:hidden gap-y-6 ml-4">
        <a href="https://web.facebook.com/abraham.abel.752/" target="_blank">
          <font-awesome-icon font-size="16" color="#fff" :icon="['fab', 'facebook']"/>
        </a>
        <a style="margin-left: 1px;" href="https://instagram.com/aybee_adayi/" target="_blank">
          <font-awesome-icon font-size="16" color="#fff" :icon="['fab', 'instagram']"/>
        </a>
        <a href="https://www.youtube.com/channel/UC4bO-Zg_yqPOdyKU_K2ZBVA/" target="_blank">
          <font-awesome-icon font-size="16" color="#fff" :icon="['fab', 'youtube']"/>
        </a>
      </div>
      <div class="h-1/6 md:h-2/6 w-0.5 ml-6 mt-6 bg-transparent md:bg-black"></div>
    </div>
    <div class="hidden md:block w-100 absolute top-2/4 left-1/4 -translate-x-2/4 -translate-y-1/4 px-24">
      <h1 class="text-white text-8xl font-bold mb-6">
        <span class="px-4 py-1" style="background-color: #70707080;">
          Aybee Adayi
        </span>
      </h1>
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
    <div class="md:hidden w-100 absolute top-3/4 right-0 -translate-y-3/4">
      <h1 class="text-white text-5xl font-bold mb-6">
        <span class="px-4 py-1" style="background-color: #70707080;">
          Aybee Adayi
        </span>
      </h1>
      <vue-typed-js
        :strings="['Creative Artist', 'Photographer', 'Videographer', 'Graphics Designer']"
        :loop="true"
        :smartBackspace='true'
        :typeSpeed='120'
        :backSpeed='50'
        :backDelay='70'
      >
        <p class="text-white text-2xl font-medium pl-4"><span class="typing"></span></p>
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
