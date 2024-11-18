<script setup>
import { ref } from 'vue';

const isNavOpen = ref(false);

const toggleNav = () => {
    isNavOpen.value = !isNavOpen.value;
}

</script>

<template>
        <a href="#home" class="logo">Tiisetso
            <span class="span">Khumalo</span>
        </a>
        

        <i class="bx bx-menu menu-icon" @click="toggleNav"></i>

        <nav  :class="[
        'navbar',
        isNavOpen ? 'flex' : 'hidden',
        'md:flex md:gap-4',
      ]">
            <a href="#home">Home</a>
            <a href="#education">Education</a>
            <a href="#services">Services</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact Me</a>
            
        </nav>
</template>