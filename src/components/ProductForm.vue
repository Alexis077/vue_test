<template>
    <form>
    <div class="form-group">
        <label>Cantidad</label>
        <input type="number" class="form-control" min="0">
    </div>
    <div class="form-group">
        <label for="exampleInputPassword1">Description</label>
        <input type="text" class="form-control">
    </div>
    <div class="form-group">
        <label>Precio unitario</label>
        <input type="number" class="form-control" min="0">
    </div>
    <button type="submit" class="btn btn-primary">Agregar</button>
    </form>
</template>

<script>
export default {
}
</script>
<style>

</style>
