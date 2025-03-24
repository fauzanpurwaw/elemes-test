<script lang="ts" setup>
defineProps({
    onTopScreen: Boolean
})
</script>
<template>
    <div class="h-[96px] flex items-center justify-between xl:mx-28 mx-4 scale-90 lg:scale-100">
        <img src="/img/elemesid.png" alt="elemes-group" class="lg:w-[200px] w-[140px] lg:h-[50px] h-[40px]">
        <div class="gap-8 text-gray font-semibold hidden lg:flex">
            <div class="cursor-pointer hover:text-black">Home</div>
            <div class="cursor-pointer hover:text-black">About</div>
            <div class="cursor-pointer hover:text-black">Promotions
                <span class="animate-pulse absolute flex -mt-9 ml-16 text-[8px] bg-[#E7462D] px-2 py-[2px] rounded-lg text-white">HOT</span>
            </div>
            <div class="cursor-pointer hover:text-black">Blogs</div>
            <div class="cursor-pointer hover:text-black">Contact Us</div>
        </div>
        <div class="flex xl:gap-8 gap-2 items-center font-semibold">
            <div class="cursor-pointer hidden lg:inline-block">Masuk</div>
            <div class="text-white text-sm! bg-primary w-[180px] h-[50px] rounded-3xl cursor-box copy">Daftar Sekarang</div>
        </div>
    </div>
</template>