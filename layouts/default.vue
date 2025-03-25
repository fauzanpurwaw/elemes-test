<script lang="ts" setup>
const { y } = useWindowScroll();
</script>
<template>
    <Nav :on-top-screen="y == 0" />
    <div class="xl:mx-28 px-3">
        <slot />
    </div>
</template>