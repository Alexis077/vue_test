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
                <td>{{product.import}}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>
<script>
export default {
    data(){
        return {
            products:[{quantity:2,description:"Ipad 128 gb",unit_price:5000,import:10000},
            {quantity:2,description:"Ipad 128 gb",unit_price:5000,import:10000},
            {quantity:2,description:"Ipad 128 gb",unit_price:5000,import:10000},
            {quantity:2,description:"Ipad 128 gb",unit_price:5000,import:10000}]
        }
    }
}
</script>

<style>
    .table{
        background-color: white;
    }
</style>
