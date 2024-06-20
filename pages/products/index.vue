<template>

    <div>
        <p>Products</p>
    
        <div v-for="p in products" v-bind:key="p.id">
        <ProductCard :product="p"/>
        </div>
    </div>                          
    
    </template>
    
    <script setup>
    
    const {data:products} = await useFetch('https://fakestoreapi.com/products');
    
    </script>
    
    <style scoped>
    
    </style>