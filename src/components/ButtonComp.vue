<template>
    <button class="flex justify-center items-center gap-2 px-7 py-4 font-monserrat text-lg leading-none bg-lt-black rounded-full text-white font-thin min-w-[200px]">
        {{  label  }}

        <img v-if="iconUrl" :src="iconUrl" />
    </button>
</template>
<script setup>
defineProps({
    label: String,
    iconUrl: String
})
</script>