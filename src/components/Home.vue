<script setup>

</script>

<template>
    <section class="home" id="home">
        <div class="home-content">
            <h1>Hi, It's <span class="span title audiowide-regular">Tiisetso</span></h1>
            <h2 class="text-animation">I'm a <span class="span title audiowide-regular"></span></h2>
            <div class="span audiowide-regular">About me</div>
            <p class="vt323-regular">I am a passionate and driven aspiring developer with a deep interest in the transformative power of technology.
                My journey began with a fascination for artificial intelligence when I first watched Iron Man, and I am committed to harnessing its potential to revolutionize healthcare.
                I aim to create innovative AI-driven solutions that make healthcare more accessible, especially in under communities.
                As I continue to explore the limitless possibilities of AI, my ambitions extend to venturing into the realms of IoT and robotics.
                I envision a future where intelligent devices seamlessly integrate with robotics to redefine industries, improve lives, and solve complex challenges.
                My goal is to merge these cutting-edge technologies to bridge the gap between healthcare and technological advancement.
            </p>

            <div class="social-icon">
                <a href="www.linkedin.com/in/tiisetso-khumalo-2802" target="_blank" rel="noopener noreferrer"><img src="/src/assets/images/icons8-linkedin-2-50.png" alt="LinkedIn icon" /></a>
                <a href="https://github.com/TiiCoder28" target="_blank" rel="noopener noreferrer"><img src="/src/assets/images/icons8-github-50.png" alt="Github icon" /></a>
            </div>
            <div class="btn-group">
                <a href="#contact" class="btn">Hire Me</a>
                <a href="#contact" class="btn">Contact Me</a>
            </div>
        </div>

        <div class="home-img">
            <img class="img-logo" src="/src/assets/images/Tiisetso Khumalo Programmer.png" />
        </div>
    </section>
</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Audiowide&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=VT323&display=swap');

.title{
    color: var(--main-color);
    font-size: 4rem;
    font-weight: 900;
    font-style: bold;
}

.audiowide-regular {
  font-family: "Audiowide", sans-serif;
  font-weight: 400;
  font-style: normal;
}


.vt323-regular {
  font-family: "VT323", monospace;
  font-weight: 400;
  font-style: normal;
}

p.vt323-regular{
    font-size: 2.5rem;
    font-weight: 400;
    line-height: 1.2;
    max-width: 1000px;
}

.social-icon img {
    width: 50px; 
    height: 50px; 
    margin: 0.2rem 0.5rem;
    transition: transform 0.3s ease, filter 0.3s ease;
}

.social-icon img:hover {
    transform: scale(1.1)translateY(5px);
    color: var(--text-color); 
    filter: brightness(0.7); 
    box-shadow: 0 0 25px var(--main-color);
    border-radius: 30%;
    background-color: var(--main-color);
}

.social-icon a {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 4.5rem;
    height: 4.5rem;
    margin: 0 30px; 
    background: transparent;
    font-size: 2.5rem;
    border-radius: 50%;
    color: var(--main-color);
    transition: 0.3s ease-in-out;
}

.img-logo{
border-radius: 50%;
box-shadow: 0 0 25px var(--main-color);
cursor: pointer;
transition: 0.4s ease-in-out;
}

.img-logo:hover{
    box-shadow: 0 0 25px var(--main-color),
                0 0 50px var(--main-color),
                0 0 100 var(--main-color);
}

@media (max-width: 768px) {
    .home {
        display: flex;
        flex-direction: column;
    }
}

section{
  min-height: 100vh;
  padding: 2.5rem 3rem;
}

.home{
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10rem;
  padding: 5rem;
  margin-left: 3rem;
}

.home-content{
  display: flex;
  flex-direction: column;
  align-items: left;
  justify-content: center;
  margin-top: 6rem;

}

.btn {
    display: inline-block;
    padding: 1rem 2.5rem;
    background-color: var(--main-color);
    box-shadow: 0 0 25px var(--main-color);
    border-radius: 1rem;
    font-size: 1.4rem;
    color: black;
    border: 2px solid transparent;
    letter-spacing: 0.1rem;
    font-weight: 600;
    transition: 0.3s ease-in-out;
    cursor: pointer;
    text-decoration: none;
    margin: 0.5rem 0.2rem;
    
}

.btn:hover{
    transform: scale(1.02);
    color: var(--text-color); 
    filter: brightness(0.7);
    box-shadow: 0 0 50px var(--main-color);
    border-radius: 10%;
    background-color: var(--main-color);
    margin: 0.4rem;
}

.btn-group a:nth-of-type(2){
    background-color: black;
    color: var(--main-color);
    border: 2px solid var(--main-color);
    box-shadow: 0 0 25px transparent;
}


.btn-group a:nth-of-type(2):hover{
    box-shadow: 0 0 25px var(--main-color);
    background-color: var(--main-color);
    color: var(--text-color)
}
.btn-group a:nth-of-type(1):hover{
    background-color: black;
    color: var(--main-color);
    border: 2px solid var(--main-color);
    box-shadow: 0 0 25px transparent
}

.text-animation{
    font-size: 34px;
    font-weight: 600;
    min-width: 280px;
}

.text-animation span{
    position: relative;
}

.text-animation span::before{
    content: "Web Developer and AI Engineer";
    color: var(--main-color);
    animation: words 20s infinite;
}

.text-animation span::after{
    content: "";
    background-color: var(--bg-color);
    position: absolute;
    width: calc(100% + 8px);
    height: 100%;
    border-left: 3px solid var(--bg-color);
    right: -8px;
    animation: cursor 0.6s infinite, typing 20s steps(14) infinite;
}

@keyframes cursor {
    to {
        border-left: 2px solid var(--main-color);
    }
}

@keyframes words {
    0%,
    20% {
        content: "Web Designer";
    }
    21%,
    40% {
        content: "Frontend Developer";
    }
    41%,
    60% {
        content: "Backend Developer";
    }
    61%,
    80%{
        content: "Software engineer";
    }
    81%,
    100%{
        content: "AI Engineer";
    }
}

@keyframes typing {
    15%,
    30%,
    45%,
    50%,
    60%,
    65%,
    75%,
    90%,
    95%,
    100%{
        width: 0;

    }
    10%,
    15%,
    20%,
    35%,
    45%,
    50%,
    60%,
    70%,
    75%,
    85%,
    90%,
    100%{
        width: calc(100% + 8);
    }
}
</style>