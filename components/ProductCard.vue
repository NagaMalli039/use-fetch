<template>
    <div>

<q-card>
<q-card-media :src="product.image"/>
<p>{{ product.title }}</p>
<img :src="product.image">
<p>{{ product.category }}</p>

<NuxtLink :to="`products/${product.id}`">

<q-btn color="amber" glossy label="View Details" />

</NuxtLink>

</q-card>
    </div>
</template>

<script setup>

const {product}= defineProps(['product'])

</script>

<style lang="scss" scoped>

</style>