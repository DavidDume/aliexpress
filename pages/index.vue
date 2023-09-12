<template>
    <MainLayout>
        <div class="mt-4 max-w-[1200px] mx-auto px-2" id="IndexPage">
            <div class="grid xl:grid-cols-6 lg:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4">
                <div v-if="products" v-for="product in products" :key="product">
                    
                    <ProductComponent :product="product" />
                </div>
            </div>
        </div>
    </MainLayout>
</template>

<script setup>
import MainLayout from '~/layouts/MainLayout.vue';

const products = [
    {id:1,title:"title", description:"desc",url:"https://picsum.photos/id/7/800/800", price:999},
    {id:31,title:"gdfgs", description:"desc",url:"https://picsum.photos/id/7/800/800", price:999},
    {id:12,title:"title", description:"desc",url:"https://picsum.photos/id/7/800/800", price:999},
    {id:15,title:"title", description:"desc",url:"https://picsum.photos/id/7/800/800", price:999},
    {id:11,title:"title", description:"desc",url:"https://picsum.photos/id/77/800/800", price:999},
    {id:5,title:"title", description:"desc",url:"https://picsum.photos/id/7/800/800", price:999},

]

</script>