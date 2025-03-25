<script lang="ts" setup>
useHead({
    title: "elemes.id"
})
</script>
<template>
    <NuxtLayout>
        <div class="sm:h-[60vh] min-h-[340px] py-4">
            <div class="h-full sm:justify-between min-h-fit sm:items-center relative">
                <div class="bg-[url('/img/body-bg.jfif')] bg-cover h-full w-full opacity-[2%]"></div>
                <div class="absolute top-0 left-0 w-full h-full lg:flex items-center justify-between">
                    <div class="max-w-[480px]">
                        <div class="text-primary sm:text-6xl text-5xl font-medium">
                            <span class="hover-underline-primary">Good Food Us</span>
                            <br>
                            <span class="hover-underline-primary">Good Mood</span>
                        </div>
                        <div class="py-4 block lg:hidden">
                            <img src="/img/food.png" alt=""
                                class="lg:h-[60vh] h-60 w-60 lg:w-full lg:p-12 p-6 bg-gray-50 rounded-full">
                        </div>
                        <div class="text-gray sm:text-md/relaxed text-sm/loose font-medium lg:pt-8">
                            I would think that conserving our natural resources should be a conservative position Not to
                            waste food, and not to throw away a lot of the food that we buy.
                        </div>
                        <div class="lg:pt-10 pt-4 flex gap-6 items-center">
                            <div class="btn-daftar cursor-box animated-button shadow-xl">Daftar Sekarang</div>
                            <div class="bg-gray-200 py-3 px-6 rounded-4xl cursor-pointer shadow-xl">About Us</div>
                        </div>
                    </div>
                    <div class="lg:py-0 py-10 hidden lg:block">
                        <img src="/img/food.png" alt=""
                            class="lg:h-[60vh] h-72 w-72 lg:w-full lg:p-12 p-8 bg-gray-50 rounded-full">
                    </div>
                </div>
            </div>
        </div>
    </NuxtLayout>
</template>