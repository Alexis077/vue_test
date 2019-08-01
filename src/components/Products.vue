<template>
    <div class="table-responsive">
        <table class="table">
            <thead>
                <tr class="text-center">
                <th scope="col">Cantidad</th>
                <th scope="col">Descripción</th>
                <th scope="col">Precio Unitario</th>
                <th scope="col">Importe</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="product of products" class="text-center">
                <th>{{product.quantity}}</th>
                <td>{{product.description}}</td>
                <td>{{product.unit_price}}</td>
                <td>{{parseFloat(product.quantity) * parseFloat(product.unit_price)}}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>
<script>
export default {
   data(){
    return {
        products:[]
    }
  },
  methods: {
    loadProducts(){
        this.axios.get('http://localhost:8082/products/').then((response) => {
            this.products = response.data.data
        })
    }
  },
  created(){
      this.loadProducts()
  }
}
</script>

<style>
    .table{
        background-color: white;
    }
</style>
