<template>
    <div>
        <header>
    <nav>

<q-toolbar-title>My Dashboard</q-toolbar-title>

<q-toolbar elevated class="bg-primary text-white">               
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="/about">About</NuxtLink> 
 <NuxtLink to="/products">Products</NuxtLink> 
</q-toolbar>
    </nav>
    </header>

    <div>  
    <slot />
  </div>

</div> 
</template>

<script setup>


</script>

<style lang="scss" scoped>

</style>