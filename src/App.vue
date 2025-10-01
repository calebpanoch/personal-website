<script setup></script>

<template>
  <div class="navbar">
    <p class="full-name">&lt;/&gt; Caleb Panoch | Software Engineer</p>
    <div class="navlinks">
      <a>Education</a>
      <a>Experience</a>
      <a class="button-link" href="CalebPanochResume.pdf">Resume</a>
    </div>
  </div>
  <div class="main">
    <div class="bio">
      <p class="intro">Hi, my name is</p>
      <p class="name">Caleb Panoch</p>
      <p class="dynamic-bio">I love to code</p>
      <p class="description">
        placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder
        placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text 
        placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text 
      </p>
      <a class="button-link-2" href="CalebPanochResume.pdf">Download CV</a>
    </div>

  </div>
  <div class="experience">
    test test test
  </div>
</template>

<style>
* {
  box-sizing: border-box;
}


html, body {
  font-family: georgia, sans-serif;
  color: #FFF;
  background: #1f1b34;
  margin: 0px;
  height: 100%;
}

.main {
  width: 100%;
  min-height: 100vh;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.experience {
  background: #2f294f;
  min-height: 50vh;
}

.bio {
  height: 100%;
  width: 40%;
  margin-top: 15vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
}
.bio p {
  margin: 0;
  padding: 5px;
}
.bio .intro{
  color: #af88ef;
  font-size: 20px;
}
.bio .name {
  opacity: .85;
  font-size: 100px;
}
.bio .dynamic-bio {
  opacity: .5;
  font-size: 60px;
}
.bio .description {
  text-align: center;
  opacity: .5;
  font-size: 20px;
  line-height: 1.5;
  padding: 20px;
}
.button-link-2 {
  font-size: 20px;
  padding: 15px;
  border: 5px solid #50055c;
  color: #fff;
  width: 200px;
  text-decoration: none;
  border-radius: 5px;
  cursor: pointer;
}
.button-link-2:hover {
  background: #af88ef;
  border: 5px solid #af88ef;
}

.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 7%;
  z-index: 9999;
  background: #1f1b34;

  padding: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  align-content: center;
  gap: 20px;
}
.navlinks {
  display: flex;
  justify-content: center;
  align-items: center;
  align-content: center;
  gap: 40px;
  padding-right: 150px;
}
.navlinks a {
  cursor: pointer;
  font-size: 20px;
}
.button-link {
  padding: 5px 10px;
  border: 5px solid #50055c;
  color: #fff;
  text-decoration: none;
  border-radius: 5px;
  cursor: pointer;
}
.button-link:hover {
  background: #af88ef;
  border: 5px solid #af88ef;
}

.navbar .full-name {
  color: #af88ef;
  font-family: georgia, sans-serif;
  margin-right: auto;
  padding-left: 40px;
  font-size: 30px;
}

@media (max-width: 1100px) {
  .navlinks {
    padding-right: 50px;
    gap: 20px;
  }

  .navlinks a {
    font-size: 10px;
  }

  .navbar .full-name {
    font-size: 20px;
    white-space: nowrap;
    padding-left: 20px;
  }

  .button-link {
    border: 2px solid #50055c;
  }
  .button-link:hover {
    background: #af88ef;
    border: 2px solid #af88ef;
  }
}

@media (max-width: 600px) {
  .navlinks {
    padding-right: 25px;
    gap: 10px;
  }

  .navlinks a {
    font-size: 5px;
  }

  .navbar .full-name {
    font-size: 11px;
    white-space: nowrap;
  }

  .button-link {
    border: 1px solid #50055c;
  }
  .button-link:hover {
    background: #af88ef;
    border: 1px solid #af88ef;
  }
}
</style>
