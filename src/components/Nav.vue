<template>
    <header class="padding-x py-8 w-full top-0">
        <div v-if="showMenu" ref="menu" class="flex bg-black fixed top-0  h-screen justify-center left-0 right-0 z-200">
            <ul class="flex flex-col w-1/3 gap-12 pt-16">
                <li v-for="item in menu" :key="item.label">
                    <a @click="toggleMenu" :href="item.href" class="text-white font-monserrat uppercase">{{ item.label }}</a>
                </li>
            </ul>
        </div>
        
        <nav class="flex justify-between items-center max-container">
            <a href="#">
                <img :src="headerLogo" width="130px" height="29px"/>
            </a>

            <ul class="flex flex-1 justify-center items-center gap-16 max-lg:hidden">
                <li v-for="item in menu" :key="item.label">
                    <a :href="item.href" class="text-lt-purple font-monserrat">{{ item.label }}</a>
                </li>
            </ul>

            <div class="hidden max-lg:block">
                <img :src="hamburger" width="25px" height="25px" @click="toggleMenu" />
            </div>
        </nav>

    </header>
</template>
<script setup>
import { ref } from 'vue';
import { headerLogo } from '../assets/images'
import { hamburger } from '../assets/icons'

const menu = [
    {
        'label': 'Home',
        href: '#home',
    },
    {
        'label': 'About us',
        href: '#about',
    },
    {
        'label': 'Services',
        href: '#services',
    },
    {
        'label': 'Contact us',
        href: '#contact',
    }
]

let showMenu = ref(false);


const toggleMenu = () => showMenu.value = !showMenu.value

</script>