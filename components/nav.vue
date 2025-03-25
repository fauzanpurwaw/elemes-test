<script lang="ts" setup>
defineProps({
    onTopScreen: Boolean
})
</script>
<template>
    <div class="h-[96px] xl:mx-28 flex text-sm items-center justify-between px-3">
        <img src="/img/elemesid.png" alt="elemes-group" class="lg:w-[180px] w-[150px] lg:h-[50px] h-[40px]">
        <div class="xl:gap-10 gap-8 text-gray hidden lg:flex font-medium text-sm">
            <div class="cursor-pointer hover:text-gray-600 hover-underline-gray">Home</div>
            <div class="cursor-pointer hover:text-gray-600 hover-underline-gray">About</div>
            <div class="cursor-pointer hover:text-gray-600 hover-underline-gray">Promotions
                <span class="animate-pulse absolute flex -mt-9 ml-16 text-[8px] bg-[#E7462D] px-2 pt-[2px] rounded-lg text-white">
                    HOT
                </span>
            </div>
            <div class="cursor-pointer hover:text-gray-600 hover-underline-gray">Blogs</div>
            <div class="cursor-pointer hover:text-gray-600 hover-underline-gray">Contact Us</div>
        </div>
        <div class="flex xl:gap-8 gap-2 items-center">
            <div class="cursor-pointer hidden lg:inline-block">Masuk</div>
            <div class="btn-daftar cursor-box animated-button font-semibold">Daftar Sekarang</div>
        </div>
    </div>
</template>