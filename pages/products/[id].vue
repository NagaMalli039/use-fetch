<template>
    <div>

        <p> {{ product.title }}</p>
        <p>{{ product.$price }}</p>
        <p>{{ product.category }}</p>
        <p> {{ product.id }}</p>
    

    </div>
</template>

<script setup>

const {id}=useRoute().params
const uri='https://fakestoreapi.com/products/'+id;

const {data: product}=await useFetch(uri);

</script>

<style lang="scss" scoped>

</style>