<script lang="ts" setup>
defineProps<{
    rate: number
}>()
</script>

<template>
    <div>
        <Icon v-for="count in 5" name="solar:star-bold" :class="[count <= rate ? 'text-amber-500' : 'text-gray-400']"
            class="hover:scale-110" />
    </div>
</template>