<template>
  <nav class="w-full relative flex items-center justify-between py-4 px-6 md:px-12">
    <span class="w-24 md:w-auto">
      <h1 class="text-1xl md:text-2xl font-semibold">Aybee
        <span class="bg-black pl-1 md:pl-4 pr-1 md:pr-4">
          <span class="text-slate-100">Adayi</span>
        </span>
      </h1>
    </span>
    <ul class="hidden md:flex">
      <li class="ml-12">
        <a href="#hero" class="text-lg font-medium">Home</a>
      </li>
      <li class="ml-12">
        <a href="#services" class="text-lg font-medium">Services</a>
      </li>
      <li class="ml-12">
        <a href="#portfolio" class="text-lg font-medium">Portfolio</a>
      </li>
      <li class="ml-12">
        <a href="#packages" class="text-lg font-medium">Packages</a>
      </li>
      <li class="ml-12">
        <a href="#testimonials" class="text-lg font-medium">Testimonials</a>
      </li>
      <li class="ml-12">
        <a href="#contact" class="text-lg font-medium">Contact</a>
      </li>
    </ul>
    <div @click="show = true" class="md:hidden cursor-pointer">
      <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="32px" height="32px" color="#000" viewBox="32 32 384.97 384.97" xml:space="preserve">
        <path d="M12.03,120.303h360.909c6.641,0,12.03-5.39,12.03-12.03c0-6.641-5.39-12.03-12.03-12.03H12.03c-6.641,0-12.03,5.39-12.03,12.03C0,114.913,5.39,120.303,12.03,120.303z"></path>
        <path d="M372.939,180.455H12.03c-6.641,0-12.03,5.39-12.03,12.03s5.39,12.03,12.03,12.03h360.909c6.641,0,12.03-5.39,12.03-12.03 S379.58,180.455,372.939,180.455z"></path>
        <path d="M372.939,264.667H132.333c-6.641,0-12.03,5.39-12.03,12.03c0,6.641,5.39,12.03,12.03,12.03h240.606 c6.641,0,12.03-5.39,12.03-12.03C384.97,270.056,379.58,264.667,372.939,264.667z"></path>
      </svg>
    </div>
    <div v-show="show" class="absolute bg-white h-screen top-0 left-0 w-full py-6 px-6 z-50">
        <svg @click="show = false" class="cursor-pointer float-right" xmlns="http://www.w3.org/2000/svg" width="32px" height="32px" viewBox="0 0 512 512">
          <path d="M256 512c141.4 0 256-114.6 256-256S397.4 0 256 0S0 114.6 0 256S114.6 512 256 512zM175 175c9.4-9.4 24.6-9.4 33.9 0l47 47 47-47c9.4-9.4 24.6-9.4 33.9 0s9.4 24.6 0 33.9l-47 47 47 47c9.4 9.4 9.4 24.6 0 33.9s-24.6 9.4-33.9 0l-47-47-47 47c-9.4 9.4-24.6 9.4-33.9 0s-9.4-24.6 0-33.9l47-47-47-47c-9.4-9.4-9.4-24.6 0-33.9z"/>
        </svg>
        <ul class="h-full w-full flex flex-col gap-8 items-center justify-center">
          <li>
            <a href="#hero" @click="show = false" class="text-lg font-medium">Home</a>
          </li>
          <li>
            <a href="#services" @click="show = false" class="text-lg font-medium">Services</a>
          </li>
          <li>
            <a href="#portfolio" @click="show = false" class="text-lg font-medium">Portfolio</a>
          </li>
          <li>
            <a href="#packages" @click="show = false" class="text-lg font-medium">Packages</a>
          </li>
          <li>
            <a href="#testimonials" @click="show = false" class="text-lg font-medium">Testimonials</a>
          </li>
          <li>
            <a href="#contact" @click="show = false" class="text-lg font-medium">Contact</a>
          </li>
        </ul>
    </div>
  </nav>
</template>
<script>
export default {
  name: 'NavMenu',
  data() {
    return {
      'show': false
    }
  },
}
</script>
<style lang="scss" scoped>
  nav {
    ul {
      li {
        a {
          position: relative;

          &::after {
            content: '';
            width: 0;
            height: 3px;
            background: #000;
            position: absolute;
            left: 0;
            bottom: -6px;
            transition: 0.5s;
          }

          &:hover::after {
            width: 100%;
          }
        }
      }
    }
  }
</style>
