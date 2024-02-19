<template>
    <section class="hero-section">
        <carousel :items-to-show="1">

          <slide v-for="slide in 1" :key="slide">
            <div class="single-hero-items set-bg" style="background-image: url('/img/model-1.jpg')">
                <div class="container">
                    <div class="row banner-info">
                        <div class="col-lg">
                            <h1>50% All Items Discount!</h1>
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
            <div class="single-hero-items set-bg" style="background-image: url('/img/models-2.jpg')">
                <div class="container">
                    <div class="row banner-info">
                        <div class="col-lg-5">
                            <!-- <span>Bag,kids</span> -->
                            <!-- <h1>Black friday</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore
                            </p> -->
                            <!-- <button class="btn primary-btn">Shop Now</button> -->
                        </div>
                    </div>
                </div>
              </div>
          </slide>
          <slide v-for="slide in 1" :key="slide">
            <div class="single-hero-items set-bg" style="background-image: url('/img/models-3.jpg')">
                <div class="container">
                    <div class="row banner-info">
                        <div class="col-lg-5">
                            <!-- <span>Bag,kids</span>
                            <h1>Black friday</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore
                            </p> -->
                            <!-- <button class="btn primary-btn">Shop Now</button> -->
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
    </section>
</template>

<script>
import "vue3-carousel/dist/carousel.css";
import {Carousel, Slide, Pagination, Navigation }  from 'vue3-carousel'

export default {
name: 'HeroMraz',
components: {
    Carousel, Slide, Pagination, Navigation
}
}
</script>

<style scoped>

h1 {
    font-size: 125px;
    font-weight :bolder;
    color: white;
}

p {
    font-size:20px;
    color:white;
}

.set-bg {
    width: 100%;
    height: 1000px;  
}

.banner-info{
    margin-top: 300px;
}
</style>