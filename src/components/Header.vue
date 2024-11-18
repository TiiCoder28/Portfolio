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

<style scoped>

.header{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 1rem 2rem;
  background: rgba(0, 0, 0, 0.3);
  backdrop-filter: blur(10px);
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  z-index: 5;

}

.span,
.logo{
  font-size: 3rem;
  color: var(--text-color);
  font-weight: 600;
  cursor: pointer;
  transition: 0.3s ease;
  text-decoration: none;
}

.logo:hover{
  transform: scale(1.1);
}

.span{
  text-shadow: 0 0 25px var(--main-color);
}
.navbar{
  display: flex;
  gap: 1rem;
}

.navbar a{
  font-size: 1.8rem;
  color: var(--text-color);
  margin-left: 4rem;
  font-weight: 500;
  transition: 0.3 ease;
  border-bottom: 3px solid transparent;
  text-decoration: none;
}

.navbar a:hover,
.navbar a:active{
  color: var(--main-color);
  border-bottom: 3px solid var(--main-color);
}

.menu-icon{
  font-size: 2rem;
  color: var(--main-color);
  display: none;
  cursor: pointer;
}

@media (max-width: 768px){
  .navbar {
    display: none;
    flex-direction: column;
    position: fixed;
    top: 4rem;
    right: 2rem;
    background: var(--second-bg-color);
    padding: 1rem 2rem;
    border-radius: 0.5rem;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
    }
    .navbar.active {
      display: flex;
    }

  .menu-icon {
    display: block;
  }
}


</style>