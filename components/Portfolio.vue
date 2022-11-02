<template>
  <div id="portfolio">
    <div class="px-14 py-20">
      <div class="w-full flex items-center justify-center">
        <span class="h-[1px] w-full bg-black"></span>
        <h3 class="text-black text-2xl md:text-5xl mx-8 font-medium">Portfolio</h3>
        <span class="h-[1px] w-full bg-black"></span>
      </div>
      <div class="px-56 mt-12">
        <div class="work__filters">
          <span @click="isActive = 'all'" :class="{ active: isActive == 'all' }" class="work__filters-item" data-filter="all">All</span>
          <span @click="isActive = 'photos'" :class="{ active: isActive == 'photos' }" class="work__filters-item" data-filter=".photos">Photos</span>
          <span @click="isActive = 'videos'" :class="{ active: isActive == 'videos' }" class="work__filters-item" data-filter=".videos">Videos</span>
          <span @click="isActive = 'graphics'" :class="{ active: isActive == 'graphics' }" class="work__filters-item" data-filter=".graphics">Graphics</span>
        </div>

        <div class="work__container">
          <div class="work__card mix photos">
            <img src="@/assets/img/c2.jpg" alt="" class="work__img">
            <h4 class="work__title">Agungu Fishing Festival</h4>
            <span class="work__button">Demo <font-awesome-icon font-size="16" icon="fa-solid fa-arrow-right" /></span>
            <div class="work__details">
              <h4 class="work__details__title"></h4>
              <p class="work_details_description"></p>
              <ul class="work__details__info">
                <li>Created - <span>1 Nov 2022</span></li>
                <li>Technologies - <span>HTML CSS</span></li>
                <li>Role - <span>Frontend</span></li>
                <li>View - <span><a href="#">www.icreated.com</a></span></li>
              </ul>
            </div>
          </div>
          <div class="work__card mix graphics">
            <img src="@/assets/img/c2.jpg" alt="" class="work__img">
            <h4 class="work__title">Agungu Fishing Festival</h4>
            <span class="work__button">Demo <font-awesome-icon font-size="16" icon="fa-solid fa-arrow-right" /></span>
            <div class="work__details">
              <h4 class="work__details__title"></h4>
              <p class="work_details_description"></p>
              <ul class="work__details__info">
                <li>Created - <span>1 Nov 2022</span></li>
                <li>Technologies - <span>HTML CSS</span></li>
                <li>Role - <span>Frontend</span></li>
                <li>View - <span><a href="#">www.icreated.com</a></span></li>
              </ul>
            </div>
          </div>
          <div class="work__card mix photos">
            <img src="@/assets/img/c2.jpg" alt="" class="work__img">
            <h4 class="work__title">Agungu Fishing Festival</h4>
            <span class="work__button">Demo <font-awesome-icon font-size="16" icon="fa-solid fa-arrow-right" /></span>
            <div class="work__details">
              <h4 class="work__details__title"></h4>
              <p class="work_details_description"></p>
              <ul class="work__details__info">
                <li>Created - <span>1 Nov 2022</span></li>
                <li>Technologies - <span>HTML CSS</span></li>
                <li>Role - <span>Frontend</span></li>
                <li>View - <span><a href="#">www.icreated.com</a></span></li>
              </ul>
            </div>
          </div>
          <div class="work__card mix graphics">
            <img src="@/assets/img/c2.jpg" alt="" class="work__img">
            <h4 class="work__title">Agungu Fishing Festival</h4>
            <span class="work__button">Demo <font-awesome-icon font-size="16" icon="fa-solid fa-arrow-right" /></span>
            <div class="work__details">
              <h4 class="work__details__title"></h4>
              <p class="work_details_description"></p>
              <ul class="work__details__info">
                <li>Created - <span>1 Nov 2022</span></li>
                <li>Technologies - <span>HTML CSS</span></li>
                <li>Role - <span>Frontend</span></li>
                <li>View - <span><a href="#">www.icreated.com</a></span></li>
              </ul>
            </div>
          </div>
          <div class="work__card mix videos">
            <img src="@/assets/img/c2.jpg" alt="" class="work__img">
            <h4 class="work__title">Agungu Fishing Festival</h4>
            <span class="work__button">Demo <font-awesome-icon font-size="16" icon="fa-solid fa-arrow-right" /></span>
            <div class="work__details">
              <h4 class="work__details__title"></h4>
              <p class="work_details_description"></p>
              <ul class="work__details__info">
                <li>Created - <span>1 Nov 2022</span></li>
                <li>Technologies - <span>HTML CSS</span></li>
                <li>Role - <span>Frontend</span></li>
                <li>View - <span><a href="#">www.icreated.com</a></span></li>
              </ul>
            </div>
          </div>
          <div class="work__card mix photos">
            <img src="@/assets/img/c2.jpg" alt="" class="work__img">
            <h4 class="work__title">Agungu Fishing Festival</h4>
            <span class="work__button">Demo <font-awesome-icon font-size="16" icon="fa-solid fa-arrow-right" /></span>
            <div class="work__details">
              <h4 class="work__details__title"></h4>
              <p class="work_details_description"></p>
              <ul class="work__details__info">
                <li>Created - <span>1 Nov 2022</span></li>
                <li>Technologies - <span>HTML CSS</span></li>
                <li>Role - <span>Frontend</span></li>
                <li>View - <span><a href="#">www.icreated.com</a></span></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Portfolio Popup -->
    <div class="portfolio__popup">

    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      isActive: "",
      mixer: null // Declare in data to avoid eslint warning
    }
  },
  mounted () {
    this.isActive = "all"
    this.$nextTick(() => {
      // const containerEl = document.querySelector('.work__container')
      // this.mixer = new this.mixitup(containerEl, {

      // })
      this.mixer = this.mixitup('.work__container')
    })
  }
}
</script>
<style lang="">

</style>
