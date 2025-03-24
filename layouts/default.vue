<script lang="ts" setup>
    const { y } = useWindowScroll();
</script>
<template>
    <Nav :on-top-screen="y == 0"/>
</template>