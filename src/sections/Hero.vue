<template>
    <section class="min-h-[70vh] hero flex justify-end max-container">
        <div class="flex w-3/5 justify-start items-center bg-gradient-to-r from-lt-purple opacity-30">
            <div class="w-3/5 max-md:w-full text-white pt-16 px-6">
                <p class="text-lg mb-2 text-xl leading-8">Cultivating growth<br/> Connecting  opportunities.</p>
                <h1 class="text-3xl max-lg:text-xl max-md:text-xl font-thin">
                Your ally in <span class="font-thin">Economic Development</span>,
                providing tailored support and expertise to foster expansion, drive job creation, and empower your team.</h1>
            </div>
        </div>
    </section>
</template>
<script setup>
import { bigShoe1, thumbnailShoe1, bigShoe2, thumbnailShoe2, bigShoe3, thumbnailShoe3 } from '../assets/images'

import { ref } from 'vue';

const shoes = [
    {
        thumbnail: thumbnailShoe1,
        bigShoe: bigShoe1,
    },
    {
        thumbnail: thumbnailShoe2,
        bigShoe: bigShoe2,
    },
    {
        thumbnail: thumbnailShoe3,
        bigShoe: bigShoe3,
    },
];

const selectedBigShoe = ref(bigShoe1)

const selectShoe = shoe => {
    selectedBigShoe.value = shoe.bigShoe
}
</script>