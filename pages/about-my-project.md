---
layout: default
title: "About My Project"
permalink: /about-my-project.html
---

<h1>About My Project</h1>

<p>Welcome to my project page! Click on each section to explore details.</p>

<div class="project-section">
  <button class="accordion">Project Title</button>
  <div class="panel">
    <p>Replace this with your project title.</p>
  </div>

  <button class="accordion">Problem</button>
  <div class="panel">
    <p>Describe the problem your project solves here.</p>
  </div>

  <button class="accordion">Approach</button>
  <div class="panel">
    <p>Explain your methodology or approach.</p>
  </div>

  <button class="accordion">Expected Outcome</button>
  <div class="panel">
    <p>What do you hope to achieve with this project?</p>
  </div>

  <button class="accordion">Final Report</button>
  <div class="panel">
    <p><a href="#" target="_blank">View Final Report (PDF)</a></p>
  </div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  var acc = document.getElementsByClassName("accordion");
  for (var i = 0; i < acc.length; i++) {
    acc[i].addEventListener("click", function () {
      this.classList.toggle("active");
      var panel = this.nextElementSibling;
      if (panel.style.maxHeight) {
        panel.style.maxHeight = null;
      } else {
        panel.style.maxHeight = panel.scrollHeight + "px";
      }
    });
  }
});
</script>

<style>
.accordion {
  background-color: #f5f5f5;
  color: #333;
  cursor: pointer;
  padding: 14px;
  width: 100%;
  text-align: left;
  border: none;
  outline: none;
  font-size: 1.1em;
  font-family: inherit;
  transition: background-color 0.3s ease;
  margin-bottom: 5px;
}

.accordion.active,
.accordion:hover {
  background-color: #e0e0e0;
}

.panel {
  padding: 0 14px;
  background-color: white;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.3s ease-out;
  border-left: 2px solid #ccc;
  margin-bottom: 8px;
}
</style>
