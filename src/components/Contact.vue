<script setup>
</script>

<template>
    <section class="contact" id="contact">
        <h3 class="heading vt323-regular">Contact Me</h3>
        <div class="timeline-items">
        <div class="timeline-item">
                <div class="timeline-dot"></div>
                    <div class="timeline-content vt323-regular">
                        <h3><img src="C:\Users\GirlCode\Desktop\Portfolio\src\assets\images\email-icon.png" alt="email-icon">Email</h3>
                        <p>You can email me on: <a href="mailto:tiisoh1998@gmail.com">tiisoh1998@gmail.com</a></p>
                    </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-dot"></div>
                    <div class="timeline-content vt323-regular">
                        <h3><img src="C:\Users\GirlCode\Desktop\Portfolio\src\assets\images\icons8-phonecall-48.png" alt="phone-icon">Contact number</h3>
                        <p>You can call me on: <a href="tel:+27670232195">+276 670 232 195</a></p>
                    </div>
            </div>
            </div>

    </section>
</template>

<style scoped>

.timeline-items{
    max-width: 1200px;
    margin: auto;
    display: flex;
    flex-wrap: wrap;
    position: relative;
}

.timeline-items::before{
    content: "";
    position: absolute;
    width: 5px;
    height: 100%;
    background-color: var(--main-color);
    left: calc(50% - 1px);

}

.timeline-item{
    margin-bottom: 50px;
    width: 100%;
    position: relative;
}

.timeline-dot{
    height: 21px;
    width: 21px;
    background-color: var(--main-color);
    box-shadow: 0 0 25px var(--main-color),
                0 0 50px var(--main-color),
                0 0 100px var(--main-color);
    position: absolute;
    left: calc(50% - 8px);
    border-radius: 50%;
    top: 5px;

}

.timeline-content{
    border: 3px solid var(--main-color);
    background-color: var(--bg-color);
    padding: 20px 40px;
    border-radius: 2.5rem;
    box-shadow: 0 0 10px var(--main-color);
    cursor: pointer;
    transition: 0.3s ease-in-out;
}

.timeline-content:hover{
    box-shadow: 0 0 25px var(--main-color);
    transform: scale(1.05);
}

.timeline-content a{
    text-decoration: none;
    color: var(--main-color);
    transition: 0.3s ease-in-out;
}

.timeline-content a:hover{
    box-shadow: 0 0 25px var(--main-color);
    transform: scale(1.05);
}


.timeline-content h3{
    font-size: 2rem;
    color: #ffffff;
    margin:  0 0 10px;
    font-weight: 500;
}

.timeline-content p{
    font-size: 1.4rem;
    line-height: 1.8rem;
}

.timeline-item:last-child{
    margin-bottom: 0;
}

.timeline-item:nth-child(odd){
    padding-right: calc(50% + 30px);
    text-align: right;
}

.timeline-item:nth-child(even){
    padding-left: calc(50% + 30px);
    text-align: left;
}


</style>