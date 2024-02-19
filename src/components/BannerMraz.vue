<template>
    <section class="women-banner spad">
        <carousel :items-to-show="3">

                            <slide v-for="slide in 1" :key="slide">
                                <div class="product-item">
                                    <div class="pi-pic">
                                        <img src="img/nike-1.png" alt="" />
                                        <ul>
                                            <li class="w-icon active">
                                                <a href="#"><i class="icon_bag_alt"></i></a>
                                            </li>
                                            <li class="quick-view"><a href="product.html">+ Quick View</a></li>
                                        </ul>
                                    </div>
                                    <div class="pi-text">
                                        <div class="catagory-name">Coat</div>
                                        <a href="#">
                                            <h5>Mickey Baggy</h5>
                                        </a>
                                        <div class="product-price">
                                            $14.00
                                            <span>$35.00</span>
                                        </div>
                                    </div>
                                </div>
                            </slide>

                            <slide v-for="slide in 1" :key="slide">
                                <div class="product-item">
                                    <div class="pi-pic">
                                        <img src="img/nike-2.png" alt="" />
                                        <ul>
                                            <li class="w-icon active">
                                                <a href="#"><i class="icon_bag_alt"></i></a>
                                            </li>
                                            <li class="quick-view"><a href="product.html">+ Quick View</a></li>
                                        </ul>
                                    </div>
                                    <div class="pi-text">
                                        <div class="catagory-name">Coat</div>
                                        <a href="#">
                                            <h5>Mickey Baggy</h5>
                                        </a>
                                        <div class="product-price">
                                            $14.00
                                            <span>$35.00</span>
                                        </div>
                                    </div>
                                </div>
                            </slide>

                            <slide v-for="slide in 1" :key="slide">
                                <div class="product-item">
                                    <div class="pi-pic">
                                        <img src="img/nike-3.png" alt="" />
                                        <ul>
                                            <li class="w-icon active">
                                                <a href="#"><i class="icon_bag_alt"></i></a>
                                            </li>
                                            <li class="quick-view"><a href="product.html">+ Quick View</a></li>
                                        </ul>
                                    </div>
                                    <div class="pi-text">
                                        <div class="catagory-name">Coat</div>
                                        <a href="#">
                                            <h5>Mickey Baggy</h5>
                                        </a>
                                        <div class="product-price">
                                            $14.00
                                            <span>$35.00</span>
                                        </div>
                                    </div>
                                </div>
                            </slide>

                            <slide v-for="slide in 1" :key="slide">
                                <div class="product-item">
                                    <div class="pi-pic">
                                        <img src="img/nike-4.png" alt="" />
                                        <ul>
                                            <li class="w-icon active">
                                                <a href="#"><i class="icon_bag_alt"></i></a>
                                            </li>
                                            <li class="quick-view"><a href="product.html">+ Quick View</a></li>
                                        </ul>
                                    </div>
                                    <div class="pi-text">
                                        <div class="catagory-name">Coat</div>
                                        <a href="#">
                                            <h5>Mickey Baggy</h5>
                                        </a>
                                        <div class="product-price">
                                            $14.00
                                            <span>$35.00</span>
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
name: 'BannerMraz',
components: {
    Carousel, Slide, Pagination, Navigation
}
}
</script>

<style scoped>

.product-item{
    margin-top:25px;
    margin-right:20px;
}

</style>