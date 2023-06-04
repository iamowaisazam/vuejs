
<script setup >
import { RouterLink } from 'vue-router';

    const breads = [
        {
            title :"Home",
            link :"/",
        },
        {
            title :">",
        },
        {
            title :"Shop",
            link :"shop",
        }
    ];

</script>
<template>

    <div class="bread">
        <div class="container">
            <div class="list">
                 <span v-for="item in breads">
                    <span v-if="item.title != '>'" >
                        <RouterLink :to="item.link">{{item.title}}</RouterLink> 
                    </span>
                    <span v-else> {{item.title}}</span>
                </span>
            </div>
        </div>
    </div>

</template>

<style scoped>

    .bread{
        background: #f0f0f0;
        padding: 30px 0px;
    }

    .bread .list a {
        color: #111;
        text-decoration: none;
        padding: 5px 8px;
        font-size: 14px;
    }

</style>