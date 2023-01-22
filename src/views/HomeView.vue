<template>
<div>
  <Banner/>
  <CategoryProducts
  :tabs="womenTabs"
  :title="womentitle"
  :products="womenProducts"/>
  <CategoryProducts
  :tabs="womenTabs"
  :title="mentitle"
  :products="womenProducts"/>
  <Featured/>
  <Subscribe/>
  <Blogs/>
  <Footer/>
</div>
</template>


<script setup>
import Banner from '../components/Banner.vue'
import CategoryProducts from '../components/CategoryProducts.vue'
import Featured from '../components/Featured.vue'
import Subscribe from '../components/Subscribe.vue'
import Blogs from '../components/Blogs.vue'
import Footer from '../components/Footer.vue'
import {ref} from 'vue'

const womenTabs = ref([
    'NEW ARRIVALS',
    'SPECIALS',
    'BESTSELLERS',
    'MOST VIEWED',
    'FEATURED PRODUCTS'

]);


const womenProducts = ref([
    {
        img: '/src/assets/images/p1.jpg',
        sale: false,
        name: 'Womens clothes',
        price: '$ 38.00',
        rating: 'src/assets/images/rating.png'
    },
     {
        img: '/src/assets/images/p1.jpg',
        sale: false,
        name: 'Womens clothes',
        price: '$ 38.00',
        rating: 'src/assets/images/rating.png'
    },
     {
        img: '/src/assets/images/p1.jpg',
        sale: false,
        name: 'Womens clothes',
        price: '$ 38.00',
        rating: 'src/assets/images/rating.png'
    },
     {
        img: '/src/assets/images/p1.jpg',
        sale: false,
        name: 'Womens clothes',
        price: '$ 38.00',
        rating: 'src/assets/images/rating.png'
    },
     {
        img: '/src/assets/images/p1.jpg',
        sale: true,
        name: 'Womens clothes',
        price: '$ 38.00',
        rating: 'src/assets/images/rating.png'
    },
     {
        img: '/src/assets/images/p1.jpg',
        sale: false,
        name: 'Womens clothes',
        price: '$ 38.00',
        rating: 'src/assets/images/rating.png'
    },
     {
        img: '/src/assets/images/p1.jpg',
        sale: false,
        name: 'Womens clothes',
        price: '$ 38.00',
        rating: 'src/assets/images/rating.png'
    },
     {
        img: '/src/assets/images/p1.jpg',
        sale: false,
        name: 'Womens clothes',
        price: '$ 38.00',
        rating: 'src/assets/images/rating.png'
    }
])

const womentitle = ref("Womens");
const mentitle = ref("Men");
</script>
