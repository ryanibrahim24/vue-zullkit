<script setup>
import ItemCard from '@/components/ItemCard.vue'
import { ref } from 'vue'

const items = ref([
    { id: 1, title: 'Mobile UI Kit', image: 'items-1.jpg', subTitle: 'Mobile UI Kit'},
    { id: 2, title: 'Online Doctor Consultation', image: 'items-2.jpg', subTitle: 'Website UI Kit'},
    { id: 3, title: 'Banking Crypto', image: 'items-3.jpg', subTitle: 'Mobile UI Kit'},
])

</script>

<template>
    <div class="container px-4 mx-auto my-16 md:px-12">
        <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">New Items</h2>
        <div class="flex flex-wrap -mx-1 lg:-mx-4">
            <ItemCard 
                v-for="item in items"
                :key="item.id"
                :id="item.id"
                :title="item.title"
                :image="item.image"
                :subTitle="item.subTitle"
            />

        </div>
    </div>
</template>