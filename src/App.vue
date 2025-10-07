<script setup>
import VueTyper from 'vue3-typer'
import "vue3-typer/dist/vue-typer.css"

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
      <a class="button-link" href="/CalebPanochResume.pdf">Resume</a>
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
      <a v-motion-roll-visible-once-left class="button-link-2" href="/CalebPanochResume.pdf">Download CV</a>
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
    <div class="box-container">
      <p class="category">Languages</p>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">HTML</p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">JavaScript</p>
      </div>
      <div v-motion-slide-visible-once-left width="auto" class="box">
        <p class="title">CSS</p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">C</p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">C++</p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">Python</p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">Lua</p>
      </div>
    </div>      
  </div>
</template>

<style></style>