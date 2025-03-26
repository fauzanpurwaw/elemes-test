<template>
    <div class="fixed bottom-0 w-full flex h-20 sm:hidden border-t border-gray-200 bg-white">
        <div class="flex w-full h-full justify-evenly">
            <div class="flex flex-col items-center justify-center w-1/4 cursor-pointer">
                <Icon name="lucide:home" class="text-primary text-2xl" />
                <span class="text-primary text-xs">Home</span>
            </div>
            <div class="flex flex-col items-center justify-center w-1/4 cursor-pointer">
                <Icon name="ph:shopping-bag" class="text-gray text-2xl" />
                <span class="text-gray-500 text-xs">Receipt</span>
            </div>
            <div class="flex flex-col items-center justify-center w-1/4 cursor-pointer">
                <Icon name="ph:user" class="text-gray text-2xl" />
                <span class="text-gray-500 text-xs">Profile</span>
            </div>
        </div>
    </div>
</template>