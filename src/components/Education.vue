<script setup>
</script>

<template>
    <section class="education vt323-regular" id="education">
        <h2 class="heading">Education</h2>

        <div class="timeline-items">
            <div class="timeline-item">
                <div class="timeline-dot"></div>
                    <div class="timeline-date">2024 - Present</div>
                    <div class="timeline-content">
                        <h3>Systems Developement - GirlCode</h3>
                        <p>A higher certificate offered by <a href="https://cms.girlcode.co.za/our-initiatives/" target="_blank" rel="noopener noreferrer">GirlCode</a> designed to young women with the skills necessary for roles in Software Developement.
                            This program provides a solid theoretical foundation and intensive practical experience in programming and database management.
                            We engage in technical projects to develop problem-solving abilities and adapt to real-world IT environments.
                            The curriculum emphasizes effective communication with IT staff and users, understanding technology's role in business, and applying problem-solving techniques in systems development.
                            By the end of the program, we are prepared to address business challenges with appropriate information technology solutions.
                        </p>
                    </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-dot"></div>
                    <div class="timeline-date">2020</div>
                    <div class="timeline-content">
                        <h3>Sports Administration - Exercise Teachers Academy</h3>
                        <p>The PlayMaker Programme, offered by <a href="https://amandladevelopment.org/" target="_blank" rel="noopener noreferrer">Amandla Safe-Hub</a>, equips young individuals with the skills necessary for careers in sports administration and community leadership.
This 12-month learnership includes a nationally recognized FET Certificate in Sport Administration (NQF Level 4), combining theoretical training and practical experience in sport management, event coordination, and facility administration.
Participants engage in hands-on projects to develop leadership and teamwork skills while organizing sports events and leading community initiatives.
The curriculum emphasizes ethical practices, financial administration, and risk management in the sports industry, preparing graduates to excel in diverse roles within sports organizations and communities.</p>
                    </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-dot"></div>
                    <div class="timeline-date">2017</div>
                    <div class="timeline-content">
                        <h3>National Senior Certificate - United Sisterhood Mitzvah School</h3>
                        <p>I obtained my National Senior certificate at United Sisterhood Mitzvah School in 2017</p>
                    </div>
            </div>
        </div>

        <h2 class="heading">Technical Certificates</h2>

        <div class="timeline-items">
            <div class="timeline-item">
                <div class="timeline-dot"></div>
                    <div class="timeline-date">2024</div>
                    <div class="timeline-content">
                        <h3>Microsoft Azure AZ-900</h3>
                        <p>The Microsoft AZ-900 certificate equips me with a foundational understanding of cloud concepts and core Azure services.
                            I gain knowledge of Azure pricing, support, and governance, as well as the basics of security and compliance within the cloud.
                            This certification prepares me to confidently explain Azure's benefits and features, making it an excellent starting point for a career in cloud computing.
                        </p>
                    </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-dot"></div>
                    <div class="timeline-date">2024</div>
                    <div class="timeline-content">
                        <h3>Microsoft Azure AI-900</h3>
                        <p>The Microsoft AI-900 certificate provides me with a solid understanding of AI concepts and Azure AI services.
                            I learn about machine learning, computer vision, natural language processing, and conversational AI.
                            This certification equips me to identify AI solutions and understand their real-world applications, making it a great foundation for diving into AI and machine learning technologies.</p>
                    </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-dot"></div>
                    <div class="timeline-date">2024</div>
                    <div class="timeline-content">
                        <h3>Microsoft Azure AI-102</h3>
                        <p>The Microsoft AI-102 certification equips me with the skills to design and implement AI solutions using Microsoft Azure.
                            I learn to build AI-driven applications that utilize Azure Cognitive Services, knowledge mining, and machine learning models.
                            This certification prepares me to create intelligent solutions, from chatbots to advanced data insights, and integrate AI seamlessly into business applications.</p>
                    </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-dot"></div>
                    <div class="timeline-date">2024</div>
                    <div class="timeline-content">
                        <h3>Microsoft Azure SC-900</h3>
                        <p>The Microsoft SC-900 certification equips me with foundational knowledge of Microsoft’s security, compliance, and identity solutions.
                            I gain insights into key principles of security, identity, and access management, as well as Microsoft’s compliance solutions.
                            This certification helps me understand how to implement these concepts across Microsoft Azure and Microsoft 365 environments.</p>
                    </div>
            </div>
        </div>

    </section>
</template>


<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Audiowide&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=VT323&display=swap');

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

.heading{
    font-size: 5rem;
    text-align: center;
    margin: 5rem 0;
}

.education{
    padding: 100px;
    background: var(--second-bg-color);
}

.education h3{
    margin-bottom: 2.5rem;
}

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

.timeline-date{
    font-size: 20px;
    font-weight: 800;
    color: #ffffff;
    margin: 6px 0 15px;
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

::-webkit-scrollbar{
    width: 15px;
}

::-webkit-scrollbar-thumb{
    background-color: var(--main-color);
}

::-webkit-scrollbar-track{
    background-color: var(--bg-color);
    width: 50px;
}
</style>