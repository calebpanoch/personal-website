<script setup>
import VueTyper from 'vue3-typer'
import "vue3-typer/dist/vue-typer.css"
</script>

<template>
  <div v-motion-slide-top class="navbar">
    <p class="full-name">&lt;/&gt; Caleb Panoch | Software Engineer</p>
    <div class="navlinks">
      <a class="button">Education</a>
      <a class="button">Experience</a>
      <a class="button-link" href="CalebPanochResume.pdf">Resume</a>
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
      <a v-motion-roll-visible-once-left class="button-link-2" href="CalebPanochResume.pdf">Download CV</a>
    </div>

  </div>
  <div class="education">
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

  <div class="experience">
    <p v-motion-slide-visible-once-bottom id="label">Experience</p>
    <div class="box-container">
      <div v-motion-slide-visible-once-left class="box">
        <p class="title">Technical Support Specialist</p>
        <p class="major">Gary Panoch Funeral Home & Cremations</p>
        <p class="date">August 2018 - Present</p>
      </div>
      <div v-motion-slide-visible-once-bottom class="box">
        <p class="title">Teaching Assistant</p>
        <p class="major">Florida Atlantic University</p>
        <p class="date">January 2024 - May 2024</p>
      </div>
      <div v-motion-slide-visible-once-right class="box">
        <p class="title">Machine Learning Internship</p>
        <p class="major">Florida Atlantic University</p>
        <p class="date">May 2023 - August 2023</p>
      </div>
    </div>      
  </div>
</template>

<style></style>