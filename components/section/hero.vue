<template>
    <div class=" sm:max-h-[480px] h-fit min-h-fit py-4">
        <div class="h-fit sm:justify-between min-h-fit sm:items-center relative">
            <div class="absolute bg-[url('/img/body-bg.jfif')] bg-cover h-full w-full -z-1 opacity-[2%]"></div>
            <div
                class="top-0 left-0 w-full h-full min-h-fit sm:flex lg:gap-20 gap-5 items-center justify-between bg-transparent">
                <div class="sm:max-w-[480px] min-w-[322px] animate-fade-in-scale">
                    <div class="text-primary lg:text-6xl text-5xl font-medium">
                        <span class="hover-underline-primary">Good Food Us</span>
                        <br>
                        <span class="hover-underline-primary">Good Mood</span>
                    </div>
                    <div class="py-4 block sm:hidden">
                        <div class="w-fit relative">
                            <img src="/img/food.png" alt=""
                                class="h-62 w-62  max-w-[360px] lg:w-full lg:p-12 p-6 bg-gray-50 rounded-full">
                            <SectionHeroBlurCardHero />
                        </div>
                    </div>
                    <div class="text-gray sm:text-md/relaxed text-sm/loose font-medium lg:pt-8 pt-4 ">
                        I would think that conserving our natural resources should be a conservative position Not to
                        waste food, and not to throw away a lot of the food that we buy.
                    </div>
                    <div class="lg:pt-10 pt-4 flex gap-6 items-center">
                        <div class="btn-daftar cursor-box animated-button shadow-xl">Daftar Sekarang</div>
                        <div class="bg-gray-200 py-3 sm:px-5 px-3 rounded-4xl cursor-pointer shadow-xl text-sm">
                            About Us</div>
                    </div>
                </div>
                <div class="max-w-[500px] sm:py-0 py-10 hidden sm:block h-full animate-fade-in-scale">
                    <div class="lg:h-full relative py-4">
                        <img src="/img/food.png" alt=""
                            class="sm:max-h-[420px]! lg:min-h-[380px] lg:min-w-[380px] min-w-[300px] w-full p-12 rounded-full bg-gray-200">
                        <SectionHeroBlurCardHero />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>