<script setup></script>

<template>
  <div class="navbar">
    <p id="full-name">&lt;/&gt; Caleb Panoch | Software Engineer</p>
    <div class="navlinks">
      <a>Education</a>
      <a>Experience</a>
      <a class="button-link">Resume</a>
    </div>
  </div>
  <div class="main">
    <p>Hi, my name is</p>
    <p>Caleb Panoch</p>
    <p>I love to code</p>
    <p>
      placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder
      placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text 
      placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text placeholder text 
    </p>
  </div>
  <div class="experience">

  </div>
</template>

<style>
* {
  box-sizing: border-box;
}


body {
  color: #FFF;
  background: #1f1b34;
  margin: 0px;
}

.main {
  text-align: center;
}

.navbar {
  padding: 10px;
  width: 100%;
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
  border: 5px solid #af88ef;
}

#full-name {
  color: #af88ef;
  font-family: georgia, sans-serif;
  margin-right: auto;
  padding-left: 40px;
  font-size: 30px;
}

@media (max-width: 1000px) {
  .navlinks {
    padding-right: 50px;
    gap: 20px;
  }

  .navlinks a {
    font-size: 10px;
  }

  #full-name {
    font-size: 20px;
    white-space: nowrap;
    padding-left: 20px;
  }

  .button-link {
    border: 2px solid #50055c;
  }
  .button-link:hover {
    border: 2px solid #af88ef;
  }
}

@media (max-width: 500px) {
  .navlinks a {
    font-size: 5px;
  }

  #full-name {
    font-size: 10px;
    white-space: nowrap;
  }

  .button-link {
    border: 1px solid #50055c;
  }
  .button-link:hover {
    border: 1px solid #af88ef;
  }
}
</style>
