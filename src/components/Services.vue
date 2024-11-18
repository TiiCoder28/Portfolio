<script setup>
import { ref } from 'vue';


const frontTechnologies = ref(['Vues.js', 'HTML', 'Javascript', 'CSS', 'Tailwind']);
const backTechnologies = ref(['Node.js', 'C#', 'Python']);
const webDesignTech = ref(['Figma', 'Canva']);
const databaseTechnologies = ref(['Firebase', 'MySQL']);


</script>

<template>
    <section class="services vt323-regular" id="services">
        <h2 class="heading">Services</h2>

        <div class="service-container">
            <div class="service-box">
                <div class="service-info">
                    <h4>Frontend Development</h4>
                    <p>
                        I specialize in building engaging and interactive web interfaces using modern technologies. 
                        From crafting seamless navigation to implementing responsive designs, 
                        I ensure that your website looks great and works flawlessly on all devices.
                        
                        <h4>Technologies</h4>
                        <ul>
                        <li v-for="(tech, index) in frontTechnologies" :key="index">{{ tech }}</li>
                    </ul>
                    </p>
                    
                    
                </div>
            </div>

            <div class="service-box">
                <div class="service-info">
                    <h4>Backend Development</h4>
                    <p>
                        I develop robust and scalable server-side solutions to power your applications. 
                        By focusing on database integration, API development, and business logic implementation, I ensure your platform runs smoothly and securely to meet your unique needs.
                    
                        <h4>Technologies</h4>
                    <p>
                        <ul>
                            <li v-for="(tech, index) in backTechnologies" :key="index">{{ tech }}</li>
                        </ul>
                    </p>
                    </p>
                    
                </div>
            </div>

            <div class="service-box">
                <div class="service-info">
                    <h4>Web Design</h4>
                    <p>
                        I craft visually appealing and user-friendly website layouts that prioritize aesthetics and functionality. 
                        My designs focus on creating intuitive navigation, responsive interfaces, and captivating visuals that enhance user experience while aligning with your brand identity.
                        <h4>Technologies</h4>
                    <p>
                        <ul>
                            <li v-for="(tech, index) in webDesignTech" :key="index">{{ tech }}</li>
                        </ul>
                    </p>
                    </p>
                    
                </div>
            </div>
            <div class="service-box">
                <div class="service-info">
                    <h4>Database management</h4>
                    <p>
                        I offer database management services that ensure your data is organized, secure, and easily accessible. From creating efficient database structures to optimizing performance,
                         I help maintain reliable and scalable data solutions that support business operations and growth.
                         <h4>Technologies</h4>
                    <p>
                        <ul>
                            <li v-for="(tech, index) in databaseTechnologies" :key="index">{{ tech }}</li>
                        </ul>
                    </p>

                        </p>
                    
                </div>
            </div>
        
        </div>
    </section>

</template>

<style scoped>

.services{
    background: var(--bg-color);
    color: black;
}

.services h2{
    margin-bottom: 5rem;
    color: #ffffff;
}

.service-container{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
    gap: 2rem;
}

.service-box{
    background-color: var(--main-color);
    min-height: 500px;
    border-radius: 2.3rem;
    border: 5px solid transparent;
    cursor: pointer;
    transition: 0.4s ease-in-out;
}

.service-box:hover{
    background: #ffffff;
    color: black;
    border: 5px solid var(--main-color);
    transform: scale(1.02);
}

.service-box .service-info{
    display: flex;
    flex-direction: column;
    text-align: left;
    max-height: 200px;
    justify-content: left;
    align-items: baseline;
    padding: 2.5rem 2.5rem;
}

.service-info h4{
    font-size: 2rem;
    font-weight: 800;
    line-height: 1;
}

.service-info p{
    font-size: 1.8rem;
    font-weight: 500;
    max-height: 100px;


}



</style>