<script setup>
</script>

<template>
    <section class="projects" id="projects">
        <h2 class="heading vt323-regular">Projects</h2>

        <div class="project-container">
            <div class="project-items-box">
                <div class="project-info">
                    <h4>Project one</h4>
                </div>
            </div>

            <div class="project-items-box">
                <div class="project-info">
                    <h4>Project Two</h4>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.project-container{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
    gap: 2rem;
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
    /* align-items: baseline; */
    padding: 3.5rem 3.5rem;
}

</style>