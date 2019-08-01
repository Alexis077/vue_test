<template>
  <div class="container">
    <Top></Top>
    <br>
    <div class="jumbotron col-md-12">
      <Products></Products>
      <ProductForm></ProductForm>
    </div>
  </div>
</template>

<script>
import Top from './components/Top';
import Products from './components/Products';
import ProductForm from './components/ProductForm';

export default {
  components:{
    Top,
    Products,
    ProductForm
  }
};
</script>
<style>
  
</style>
