<template>
    <section class="women-banner spad">
        <!-- <div class="col-lg-12 mt-5" v-if="products.length > 0"> -->
            <carousel ref="product" :items-to-show="1" v-if="products.length > 0">

                                <slide v-for="slide in 1" :key="slide">
                                    <div class="product-item" v-for="itemProduct in products" v-bind:key="itemProduct.id">
                                        <div class="pi-pic">
                                            <img v-bind:src="itemProduct.galleries[0].photo" alt="" />
                                            <ul>
                                                <li class="w-icon active">
                                                    <a href="#"><i class="icon_bag_alt"></i></a>
                                                </li>
                                                <li class="quick-view">
                                                    <router-link v-bind:to="'/product/'+itemProduct.id">+ Quick View</router-link>
                                                </li>
                                            </ul>
                                        </div>
                                        <div class="pi-text">
                                            <div class="catagory-name">{{itemProduct.type}}</div>
                                            <router-link to="/product"><a href="#">
                                                <h5>{{itemProduct.name}}</h5>
                                            </a>
                                            </router-link>
                                            <div class="product-price">
                                                Rp. {{itemProduct.price}}
                                                <span>Rp.350.000</span>
                                            </div>
                                        </div>
                                    </div>
                                </slide>

                                <!-- <slide v-for="slide in 1" :key="slide">
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
                                </slide>     -->

                                <template #addons>
                                <navigation />
                                <pagination />
                            </template>
        </carousel>
    <!-- </div> -->
    <div class="col-lg-12" v-else>
        <p>
            Produk terbaru belum tersedia.
        </p>
    </div>
    </section>
</template>

<script>
import "vue3-carousel/dist/carousel.css";
import axios from "axios";
import {Carousel, Slide, Pagination, Navigation }  from 'vue3-carousel'
// import {ref} from 'vue';

// const product = ref(null);

// if (product.data.currentSlide === 1 ){
    
// }

export default {
    name: 'BannerMraz',
    components: {
        Carousel, Slide, Pagination, Navigation
    },
    data(){
        return{
            products: []
        };
    },
    mounted() {
        axios
        .get("http://127.0.0.1:8000/api/products")
        .then(res =>(this.products = res.data.data.data))
        .catch(err => console.log(err));
    }
};
</script>

<style scoped>

.product-item{
    margin-top:25px;
    margin-right:20px;
}

</style>