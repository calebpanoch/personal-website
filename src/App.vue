<script setup>
import VueTyper from 'vue3-typer'
import "vue3-typer/dist/vue-typer.css"
const languages = ["Python", "C/C++", "JavaScript", "SQL", "LUA"]
const fwstls = ["TensorFlow", "NumPy", "GCP", "Git", "Back4App", "HTML5", "CSS", "React", "Node.js"]
const concepts = ["Machine Learning", "AI-driven Systems", "Scalable Web Development", "Cloud Deployment", "Data Analysis", "Automation"]

function scrollTo(id) {
  const el = document.getElementById(id)
  if (el) {
    el.scrollIntoView({ behavior: 'smooth' })
  }
}
</script>

<template>
  <div v-motion-slide-top class="navbar">
    <p class="full-name">&lt;/&gt; Caleb Panoch | Software Engineer</p>
    <div class="navlinks">
      <a class="button" @click.prevent="scrollTo('education')">Education</a>

      <a class="button" @click.prevent="scrollTo('experience')">Experience</a>
      <a class="button-link" href="/CalebPanochResume.pdf" target="_blank">Resume</a>
    </div>
  </div>
  <div class="main">
    <div v-motion-slide-visible-once-top class="bio">
      <p v-motion-roll-visible-once-left class="intro">Hi, my name is</p>
      <p v-motion-roll-visible-once-right class="name">Caleb Panoch</p>
      
      <p v-motion-roll-visible-once-left class="dynamic-bio">
        <VueTyper 
          :text="['I\'m a lifelong learner in tech. ', 'I thrive on solving puzzles. ', 'I love to fish! ']"
          eraseStyle="backspace"
          erase-delay='50'
          style="color: #fff;"
          preEraseDelay="4000"
        />
      </p>
      <p v-motion-roll-visible-once-right class="description">
        I'm a recent M.S. graduate in Computer Science from Florida Atlantic University 
        with nearly a decade of coding experience. I'm passionate about building efficient software, 
        solving real-world problems, and alway learning new technologies. I'm now seeking opportunities 
        where I can contribute my skills and grow as a software engineer.
      </p>
      <a v-motion-roll-visible-once-left class="button-link-2" href="/CalebPanochResume.pdf" target="_blank">Download CV</a>
      <div class="links-container">
        <a href="https://github.com/calebpanoch"><img style="height: 60px;" src="/github-mark.png"></a>
        
        <a href="https://www.linkedin.com/in/calebpanoch/"><img style="height: 60px;" src="/linkedin-mark.png"></a>
      </div>
    </div>

  </div>
  <div class="education" id="education">
    <p v-motion-slide-visible-once-bottom id="label">Education</p>
    <div class="box-container">
      <div v-motion-slide-visible-once-left class="box">
        <p class="title">Florida Atlantic University</p>
        <p class="major">Bachelor of Science in Computer Science</p>
        <p class="date">August 2020 - December 2023</p>
        <p class="gpa">GPA: 3.95</p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">Florida Atlantic University</p>
        <p class="major">Masters of Science in Computer Science</p>
        <p class="date">January 2024 - December 2024</p>
        <p class="gpa">GPA: 3.9</p>
      </div>
    </div>      
  </div>

  <div class="experience" id="experience">
    <p v-motion-slide-visible-once-bottom id="label">Experience</p>
    <div class="box-container">
      <div v-motion-slide-visible-once-left class="box">
        <p class="title">Technical Support Specialist</p>
        <p class="major">Gary Panoch Funeral Home & Cremations</p>
        <p class="date">August 2018 - Present</p>
        <p class="description">Provided technical support and information about computer and tablet devices. Also set up live streaming service for families at home during the pandemic.</p>
      </div>
      <div v-motion-slide-visible-once-bottom class="box">
        <p class="title">Teaching Assistant</p>
        <p class="major">Florida Atlantic University</p>
        <p class="date">January 2024 - May 2024</p>
        <p class="description">Taught students Theory of Computation and graded assignments.</p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">Machine Learning Internship</p>
        <p class="major">Florida Atlantic University</p>
        <p class="date">May 2023 - August 2023</p>
        <p class="description">Worked with Dr. Zhen Ni to predict future energy usage of smart buildings based on previous recorded data using different Machine Learning techniques.</p>
      </div>
    </div>      
  </div>

  <div class="education" id="skills">
    <p v-motion-slide-visible-once-bottom id="label">Skills</p>
    <div>
      <p class="category">Languages</p>
      <div class="box-row">
        <div
          v-for="(language, index) in languages"
          :key="index"
          v-motion-slid-visible-once-left
          class="box"
          >
          <p class="title">{{ language }}</p>
        </div>
      </div>

      <p class="category">Frameworks/Tools</p>
      <div class="box-row">
        <div
          v-for="(fwtl, index) in fwstls"
          :key="index"
          v-motion-slid-visible-once-left
          class="box"
          >
          <p class="title">{{ fwtl }}</p>
        </div>
      </div>

      <p class="category">Concepts</p>
      <div class="box-row">
        <div
          v-for="(concept, index) in concepts"
          :key="index"
          v-motion-slid-visible-once-left
          class="box"
          >
          <p class="title">{{ concept }}</p>
        </div>
      </div>
      <br></br>
      <br></br>
      <br></br>
      <br></br>
    </div> 
  </div>
  <div class="experience" id="projects">
    <p v-motion-slide-visible-once-bottom id="label">Projects</p>
    <div class="box-container">
      <div v-motion-slide-visible-once-left class="box">
        <p class="title">Autonomous Receptionist Robot Dog</p>
        <p class="major">Installed facial recognition python packages on a robot dog that can retrieve your appointment information from a
database. Then the robot dog leads you to your appointment location</p>
      </div>
      <div v-motion-slide-visible-once-left class="box">
        <p class="title">Fish Finder Website</p>
        <p class="major">Built a full-stack fishing spot discovery app using React with an interactive map interface (Google Maps style plugin),
backed by a Node.js/Express API, enabling users to upload, browse, and tag fishing locations.<br></br><br></br> Also implemented cloud-native architecture on Google Cloud Platform, including Cloud Storage buckets for image handling and GCP hosting for the frontend/backend, optimizing performance, scalability, and deployment workflows</p>
        <p class="date"><a style="color: #af88ef" href="https://findfish.dev">FindFish.dev</a></p>
      </div>
      <div v-motion-slide-visible-once-bottom class="box">
        <p class="title">FAU Social Board</p>
        <p class="major">
          Developed a full-stack social web app enabling user registration, login, and post sharing using HTML, CSS, and JavaScript.
          <br></br><br></br>
          Implemented scalable frontend logic and optimized data flow to enhance user engagement and responsiveness.</p>
        <p class="date"><a style="color: #af88ef" href="https://github.com/calebpanoch/cen4010_spr23_g20">GitHub</a></p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">JPG Image Sharing Website Using CI/CD</p>
        <p class="major">
          Built and deployed a cloud-based image sharing platform using Google Cloud services and CI/CD pipelines.
          <br></br><br></br>
          Utilized Google Cloud Storage for image management and Datastore for metadata persistence, with secure
          authentication through Back4App.
        </p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">Multi-Party Computation Intersection</p>
        <p class="major">
          Developed a GUI application that uses cryptographic protocols to compare datasets across distributed instances without exposing private data.
          <br></br><br></br>
          Demonstrated secure computation principles in multi-user environments.
        </p>
      </div>
    </div>      
  </div>

</template>

<style></style>