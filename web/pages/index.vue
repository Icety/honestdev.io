
<script setup lang="ts">
import { ref } from 'vue';
import { useAppStore } from '@/stores/index';
const store = useAppStore();

const activeTab = ref('all');
</script>


<template>
  <div>
    <div class="relative overflow-hidden bg-black pt-[82px] sm:-mx-[250px] sm:rounded-b-[50%] lg:-mx-[150px] lg:pt-[106px]">
      <div class="relative">
        <img src="/assets/images/banner-lefticon.png" alt="banner-lefticon" class="absolute left-0 top-20 sm:left-[250px] lg:left-[150px]" />
        <img src="/assets/images/banner-rightIcon.png" alt="banner-rightIcon" class="absolute right-0 -top-4 sm:right-[250px] lg:right-[150px]" />
        <div class="container">
          <div class="relative bg-[url('/assets/images/world-map.png')] bg-cover bg-top bg-no-repeat pt-14 pb-0 lg:pt-20 lg:pb-60 xl:pt-36">
            <div class="relative z-[1] text-center text-white lg:w-3/5 ltr:lg:text-left rtl:lg:text-right xl:w-1/2">
              <h2 class="text-4xl font-extrabold leading-normal sm:text-5xl lg:text-[65px] lg:leading-[90px]">
                Building <span class="italic text-primary">Trust </span> with <span class="italic text-secondary">Transparent</span> solutions
              </h2>
              <p class="my-8 text-lg lg:w-[90%]">
                Honest pricing, fair projects, clear communication, reliable results.
              </p>
<!--              <NuxtLink to="/about-us" class="btn mx-auto mt-2 block w-fit bg-white lg:mx-0 lg:rtl:ml-auto">read more</NuxtLink>-->
            </div>
            <div
                class="bottom-0 mx-auto mt-5 mb-2 w-auto ltr:right-0 rtl:left-0 md:w-[540px] lg:absolute lg:mb-0 lg:mt-0 xl:w-[650px]"
                :data-aos="store.direction === 'rtl' ? 'fade-right' : 'fade-left'"
                data-aos-duration="1000"
                data-aos-offset="0"
                data-aos-delay="300"
            >
              <img src="/assets/images/home-banner-icon.svg" alt="home-banner-icon" class="rtl:rotate-y-180" />
            </div>
          </div>
        </div>
      </div>
    </div>

    <section class="bg-[url(/assets/images/service-bg.png)] bg-cover bg-center bg-no-repeat py-14 dark:bg-none lg:py-[100px]">
      <div class="container">
        <div class="heading text-center">
          <h6>More coming soon</h6>
          <h4>Exciting....</h4>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>

</style>
