<script setup>
import { RouterLink } from 'vue-router';


</script>
<template>
 
        <ul>
           <li class="text-danger" ><RouterLink to="/">Home</RouterLink></li>
           <li><RouterLink to="/about">About</RouterLink></li>
           <li><RouterLink to="/contact">Contact</RouterLink></li>
        </ul>
</template>