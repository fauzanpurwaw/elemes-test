<script lang="ts" setup>
// Create 10 slides
import { categories } from '../../storage.json';
const containerRef = ref<any>(null)
const slides = ref(categories)

const swiper = useSwiper(containerRef)
</script>

<template>
    <div class="xl:mx-auto lg:mx-20 sm:px-5 sm:max-w-[1280px] animate-fade-in-scale" v-if="categories">
        <div class="flex flex-col sm:px-0 px-8 gap-3 mt-20">
            <div class="text-3xl font-semibold hover-underline-black w-fit">Browse Our Category</div>
            <div class="text-primary text-3xl font-semibold hover-underline-primary w-fit">Receipt</div>
        </div>
        <ClientOnly>
            <swiper-container ref="containerRef" class="swiper-container sm:h-[220px] h-48 mt-10"
                :slides-per-view="'auto'" :space-between="10">
                <swiper-slide v-for="(slide, idx) in slides" :key="idx"
                    class="swiper-slide rounded-lg sm:first:mx-0 first:mx-8 h-44 w-62! hover:h-48 transition-all duration-300 cursor-pointer"
                    :style="{
                        backgroundColor: slide.color,
                    }">
                    <div class="flex flex-col items-center justify-center gap-1">
                        <img :src="slide.iconPath" alt="" srcset="" class="h-12 w-12 mx-auto">
                        <div class="text-lg font-medium">{{ slide.name }}</div>
                        <div class="text-sm">{{ slide.items }} Items</div>
                    </div>
                </swiper-slide>
            </swiper-container>
        </ClientOnly>

        <div class="gap-4 justify-end hidden sm:flex">
            <!-- Go back one slide -->
            <button
                class="btn-daftar cursor-box h-fit! w-fit! animated-button shadow-xl flex cursor-pointer hover:-translate-0.5 duration-200 items-center gap-2 bg-primary text-white px-4! py-2! rounded-full"
                @click="swiper.prev()">
                Prev
                <Icon name="tabler:circle-chevron-left-filled" class="bg-white text-2xl" />
            </button>
            <!-- Go forward one slide -->
            <button
                class="btn-daftar cursor-box h-fit! w-fit! animated-button shadow-xl flex cursor-pointer hover:-translate-y-0.5 hover:translate-x-0.5 duration-200 items-center gap-2 bg-primary text-white px-4! py-2! rounded-full"
                @click="swiper.next()">
                Next
                <Icon name="tabler:circle-chevron-right-filled" class="bg-white text-2xl" />
            </button>
        </div>
    </div>
</template>

<style scoped>
.swiper-slide {
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 24px;
    background-color: #f0f0f0;
    color: #333;
    z-index: 9999;
}

.swiper-button {
    margin-top: 20px;
    padding: 10px 20px;
    background-color: #8BAC3E;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
</style>