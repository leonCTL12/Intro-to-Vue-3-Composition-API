<script setup>
import {ref} from 'vue'
import socksGreenImage from './assets/images/socks_green.jpeg'
import socksBlueImage from './assets/images/socks_blue.jpeg'

const product = ref('Boots')
const description =ref('whatever description this socks is bad')
const image = ref(socksGreenImage)
const url = ref("https://github.com/")

</script>

<template>
  <div class="product-display">
    <div class="product-container">
      <div class="product-image">
        <img :src="image" alt="Product Image" />
      </div>
      <div class="product-info">
        <h1>{{ product }}</h1>
        <p>{{ description }}</p>
      </div>

      <a :href="url">A link!</a>
      
    </div>
  </div>
</template>