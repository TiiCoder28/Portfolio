<script setup>
</script>

<template>
    <section class="projects" id="projects">
        <h2 class="heading vt323-regular">Projects</h2>

   
        <div class="timeline-items">
        <div class="timeline-item">
                    <div class="timeline-content vt323-regular">
                        <h4>Weather Application</h4>
                        <a href="https://tiicoder28.github.io/weatherApp/">Weather application</a>
                        <p> This project was coded using HTML, CSS and JS. Here I use a lot of Asynchronous Javascript functions, I am also using an API from the OpenWeather site 
                        for finding the of the provided location and I am also using the geolocation API for finding the user's location
                        </p>
                
                    </div>
            </div>
            </div>
    </section>
</template>

<style scoped>

.projects{
    background-color: var(--second-bg-color);
    padding: 100px;
}

h4{
    font-size: 5rem;
    color: #ffffff;
    margin:  0 0 10px;
    font-weight: 500;
}


a{
    font-size: 2rem;
    color: var(--bg-color);
    transition: 0.3s ease-in-out;

}

a:hover{
    box-shadow: 0 0 25px var(--main-color);
    transform: scale(1.05);
}
.project-container{
    display: flex;
    justify-content: center;
    align-items: center;

}

.project-items-box{
    background-color: var(--main-color);
    min-height: 200px;
    border-radius: 2.3rem;
    border: 5px solid transparent;
    cursor: pointer;
    transition: 0.4s ease-in-out;
}

.project-items-box:hover{
    background: #ffffff;
    color: black;
    border: 5px solid var(--main-color);
    transform: scale(1.02);
}

.project-items-box .project-info{
    display: flex;
    flex-direction: column;
    text-align: left;
    max-height: 200px;
    justify-content: left;
    padding: 3.5rem 3.5rem;
}


p{
    font-size: 1.8rem;
}
</style>