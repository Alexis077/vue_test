<template>
  <div class="container">
    <navigation></navigation>
    <br>
    <top></top>
    <br>
    <div class="jumbotron col-md-12">
      <products></products>
    </div>
  </div>
</template>

<script>
import top from './components/top.vue';
import products from './components/products.vue';
import navigation from './components/navigation.vue';

export default {
  components:{
    top,
    products,
    navigation
  }
};
</script>