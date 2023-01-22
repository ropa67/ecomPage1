<template>
   <section class="category-products">
       <div class="container">
           <CategoryHeader :title="title" :tabs="tabs"/>
               <div class="products">
                   <SingleProduct
                   v-for="product in products"
                   :key="product"
                   :product="product"
                   />
               </div>
               <button class="btn">SEE ALL</button>
       </div>
    </section>
</template>

<script setup>
import { defineProps} from "vue";
import SingleProduct from './SingleProduct.vue'
import CategoryHeader from './CategoryHeader.vue'

defineProps(['title', 'products', 'tabs'])

</script>

<style scoped>

.category-products {
  margin-bottom: 100px;
}
.category-products .btn {
  height: 48px;
  background: #f8f8f8;
  border: 2px solid #f8f8f8;
  max-width: 100%;
  margin-top: 18px;
}
.products {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  gap: 30px;
}

@media (max-width: 969px) {
  .products {
    grid-template-columns: 1fr 1fr;
  }
}
@media (max-width: 400px) {
  .products {
    grid-template-columns: 1fr;
  }
}
</style>
