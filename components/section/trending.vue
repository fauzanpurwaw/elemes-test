<script lang="ts" setup>
import { trending, categories } from '../../storage.json';

const getCategoryColor = (name: string): string | undefined => {
    return categories.find((category: any) => category.name === name)?.color;
}
</script>

<template>
    <div class="flex h-full w-full mt-20">
        <div class="flex flex-col gap-3">
            <div class="text-3xl font-semibold hover-underline-black w-fit">Browse Our Trending</div>
            <div class="text-primary text-3xl font-semibold hover-underline-primary w-fit">Receipt</div>
        </div>
    </div>
    <div class="grid w-full justify-between mt-10 xl:grid-cols-4 lg:grid-cols-3 sm:grid-cols-2 grid-cols-1 gap-5">
        <div v-for="(data, idx) in trending" :key="idx"
            class="w-full h-64 min-w-64 rounded-2xl p-5 flex flex-col gap-3 cursor-pointer"
            :style="{ backgroundColor: getCategoryColor(data.category) }">
            <img :src="`/img/${data.name}.png`" alt="" class="h-32 w-32">
            <div class="flex flex-col">
                <div class="font-semibold text-lg">{{ data.name }}</div>
                <div class="font-semibold text-primary text-sm">{{ data.category }}</div>
                <Rating :rate="data.rating" />
            </div>
        </div>
    </div>
    <div class="flex w-full justify-center my-20">
        <div class="btn-daftar cursor-box animated-button shadow-xl">ALL Receipt</div>
    </div>
</template>