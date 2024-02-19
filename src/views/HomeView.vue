<template>
  <div class="home">
    <HeaderMraz />
    <HeroMraz />
    <BannerMraz />
    <InstaMraz />
    <PartnerMraz />
    <FooterMraz />

    <!-- <section class="hero-section">
        <carousel :items-to-show="1">

          <slide v-for="slide in 1" :key="slide">
            <div class="single-hero-items set-bg" style="background-image: url('/img/hero-1.jpg')">
                <div class="container">
                    <div class="row banner-info">
                        <div class="col-lg-5">
                            <span>Bag,kids</span>
                            <h1>Black friday</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore
                            </p>
                            <button class="btn primary-btn">Shop Now</button>
                        </div>
                    </div>
                </div>
              </div>
          </slide>
          <slide v-for="slide in 1" :key="slide">
            <div class="single-hero-items set-bg" style="background-image: url('/img/hero-2.jpg')">
                <div class="container">
                    <div class="row banner-info">
                        <div class="col-lg-5">
                            <span>Bag,kids</span>
                            <h1>Black friday</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore
                            </p>
                            <button class="btn primary-btn">Shop Now</button>
                        </div>
                    </div>
                </div>
              </div>
          </slide>
          <slide v-for="slide in 1" :key="slide">
            <div class="single-hero-items set-bg" style="background-image: url('/img/hero-3.jpg')">
                <div class="container">
                    <div class="row banner-info">
                        <div class="col-lg-5">
                            <span>Bag,kids</span>
                            <h1>Black friday</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore
                            </p>
                            <button class="btn primary-btn">Shop Now</button>
                        </div>
                    </div>
                </div>
              </div>
          </slide>
          <template #addons>
            <navigation />
            <pagination />
        </template>

      </carousel>
    </section> -->

  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
// import "vue3-carousel/dist/carousel.css";
// import {Carousel, Slide, Pagination, Navigation }  from 'vue3-carousel'
import HeaderMraz from '@/components/HeaderMraz.vue';
import HeroMraz from'@/components/HeroMraz.vue';
import BannerMraz from '@/components/BannerMraz.vue';
import InstaMraz from '@/components/InstaMraz.vue';
import PartnerMraz from '@/components/PartnerMraz.vue';
import FooterMraz from '@/components/FooterMraz.vue';


export default {
  name: 'HomeView',
  components: {
    HeaderMraz,
    HeroMraz,
    BannerMraz,
    InstaMraz,
    PartnerMraz,
    FooterMraz
    // Carousel, Slide, Pagination, Navigation
  }
}
</script>

