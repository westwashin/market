<template>
<div class="partner-logo">
    <carousel :items-to-show="5">
                <slide v-for="slide in 1" :key="slide">
                    <div class="logo-item">
                        <div class="tablecell-inner">
                            <img src="img/logo-carousel/logo-1.png" alt=""/>
                        </div>
                    </div>
                </slide>
                <slide v-for="slide in 1" :key="slide">
                    <div class="logo-item">
                        <div class="tablecell-inner">
                            <img src="img/logo-carousel/logo-2.png" alt=""/>
                        </div>
                    </div>
                </slide>
                <slide v-for="slide in 1" :key="slide">
                    <div class="logo-item">
                        <div class="tablecell-inner">
                            <img src="img/logo-carousel/logo-3.png" alt="" />
                        </div>
                    </div>
                </slide>
                <slide v-for="slide in 1" :key="slide">
                    <div class="logo-item">
                        <div class="tablecell-inner">
                            <img src="img/logo-carousel/logo-4.png" alt="" />
                        </div>
                    </div>
                </slide>
                <slide v-for="slide in 1" :key="slide">
                    <div class="logo-item">
                        <div class="tablecell-inner">
                            <img src="img/logo-carousel/logo-5.png" alt="" />
                        </div>
                    </div>
                </slide>
            <!-- <template #addons>
                <navigation />
                <pagination />
            </template> -->
    </carousel>
</div>
</template>

<script>
import "vue3-carousel/dist/carousel.css";
import {Carousel, Slide}  from 'vue3-carousel'

export default {
    name: 'PartnerMraz',
    components: {
    Carousel, Slide
}
}

</script>