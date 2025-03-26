<script lang="ts" setup>
import { categories } from '../storage.json';
</script>
<template>
    <div class="flex w-full mt-50 gap-4 flex-wrap sm:mb-0 mb-28">
        <div class="flex flex-col gap-3 w-96">
            <img src="/img/elemesid.png" alt="" class="w-[200px] h-14">
            <div class="text-sm text-gray  mt-1">
                Jl. Prof. DR. Satrio No.7, RT.3/RW.3, Karet Kuningan,
                Kecamatan Setiabudi, Kota Jakarta Selatan,
                Daerah Khusus Ibukota Jakarta 12950.
            </div>
            <div class="flex gap-4 my-2">
                <div
                    class="bg-white rounded-full flex justify-center items-center p-3 group hover:bg-primary transition-all duration-600 cursor-pointer">
                    <Icon name="lucide:mail"
                        class="text-primary group-hover:text-white text-xl group-hover:rotate-y-[360deg] duration-300 transition-all" />
                </div>
                <div
                    class="bg-white rounded-full flex justify-center items-center p-3 group hover:bg-primary transition-all duration-600 cursor-pointer">
                    <Icon name="ph:phone"
                        class="text-primary group-hover:text-white text-xl group-hover:rotate-y-[360deg] duration-300 transition-all" />
                </div>
                <div
                    class="bg-white rounded-full flex justify-center items-center p-3 group hover:bg-primary transition-all duration-600 cursor-pointer">
                    <Icon name="hugeicons:instagram"
                        class="text-primary group-hover:text-white text-xl group-hover:rotate-y-[360deg] duration-300 transition-all" />
                </div>
            </div>
        </div>
        <div class="flex flex-col gap-3 pr-20">
            <div class="text-lg font-medium">
                Categories
            </div>
            <div class="flex flex-col gap-3 my-4">
                <div v-for="category in categories" class="hover-underline-black cursor-pointer text-gray w-fit!">{{
                    category.name }}</div>
            </div>
        </div>
        <div class="flex flex-col gap-3 pr-20">
            <div class="text-lg font-medium">
                About Us
            </div>
            <div class="flex flex-col gap-3 my-4">
                <div class="hover-underline-black cursor-pointer text-gray w-fit!">About Us</div>
                <div class="hover-underline-black cursor-pointer text-gray w-fit!">FAQ</div>
                <div class="hover-underline-black cursor-pointer text-gray w-fit!">Report Problem</div>
            </div>
        </div>
        <div class="flex flex-col gap-3 ">
            <div class="text-lg font-medium">
                Newsletter
            </div>
            <div class="text-sm text-gray mt-4 w-72">
                Get now free 50% discount for alll products on your first order
            </div>
            <div class="flex h-12 items-center">
                <input type="email" placeholder="Your email address"
                    class="border border-gray-300 p-2 w-full rounded-l-md h-full text-gray-600 focus:outline-none" />
                <button class="bg-primary h-full text-white px-4 rounded-r-md cursor-pointer">SEND</button>
            </div>
            <div class="flex flex-col gap-2">
                <div class="flex items-center gap-2 cursor-pointer">
                    <Icon name="lucide:mail" class="text-primary text-xl" />
                    <span class="text-black hover:underline">elemesid@gmail.com</span>
                </div>
                <div class="flex items-center gap-2 cursor-pointer">
                    <Icon name="ph:phone" class="text-primary text-2xl" />
                    <span class="text-black hover:underline -ml-0.5">0888 1111 2222</span>
                </div>
            </div>
        </div>
    </div>
</template>