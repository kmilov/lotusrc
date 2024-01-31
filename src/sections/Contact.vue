<template>
    <section class="max-container flex flex-row items-center justify-center">
        <div class="bg-lt-orange p-12 w-1/2 max-md:w-full">
            <h1 class="text-3xl text-white mb-10">Contact us</h1>
            <div id="form"></div>
        </div>
    </section>
</template>

<script setup>
hbspt.forms.create({
    region: "eu1",
    portalId: "143650862",
    formId: "d44a896f-0d1d-4a3c-8ce1-58fedb8d0158",
    target:  '#form'
});
</script>