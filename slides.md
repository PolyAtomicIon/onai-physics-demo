---
theme: apple-basic
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## 29Digits
  Interactive Solutions

  Learn more at [29Digits Studio](https://t.me/digit29)

drawings:
  persist: false
css: unocss
title: Welcome to lesson
---

# Force

What is force?

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Let's start <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/PolyAtomicIon/onai-physics-demo" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
---
<SimIframe 
  src='https://codepen.io/usefulthink/full/YNrvpY'
  :applyStyle="false"
  height="470px"
/>

---

### Force: pushing, pulling anfdgdfgdfgd springs!
<br>
<SimIframe 
  src="https://brm.io/matter-js/demo/#slingshot"
  height="400px"
  width="300px"        
/>


---
---
### Same stuff, but in 3d ?!
<SimIframe
  src='https://threejs.org/examples/physics_ammo_rope.html'
  height="450px"
  :applyStyle="false"
/>
---
---

# What is Force?


- **Force** is any push or pull.
- Unit of Force is **Newton [N]**

<br>
<br>

## 3 types of Force:
- Gravitational Force
- Elastic Force
- Frictional Force

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1, h2 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
 ul li {
 	font-size: 24px;
  }
</style>

<!--
Here is another comment.
-->

---

# 1. Gravitational Force

Mutual Force of attraction between any two objects in the Universe.

$\vec{\mathbf{W}}=m\times\vec{\mathbf{G}}$\
<br/>
$\vec{\mathbf{W}} - weight [N]$\
$m - mass [kg]$\
$\vec{\mathbf{G}} - accelration\: of\: Gravity\: [m / s^2]\: or\: [N / kg]$\

<style>
h1, h2, h3 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>
---
---
### Sim of gravity

<SimIframe 
  src="https://phet.colorado.edu/sims/html/gravity-and-orbits/latest/gravity-and-orbits_en.html"
  :applyStyle="false"
  height="450px"
/>

<style>
h1, h2, h3 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

<SimIframe 
  src="https://lab.nationalmedals.org/gravity.php"
  height="470px"
  width="100%"
  :applyStyle="false"
/>


---
layout: image-right
image: >-
  https://content.osgnetworks.tv/gameandfishing/content/photos/gaf-ATABestCompounds-Lead-1200x800.jpg
---

# 2. Elastic Force

Mutual Force of attraction between any two objects in the Universe.

$\vec{\mathbf{F}}=k\times \vec{\triangle\mathbf{l}}$\
<br/>
$\vec{\mathbf{F}}$ - Force of spring [N]
$\\k$ - spring constant [N/m]
$\\\vec{\triangle\mathbf{l}}$ - extension or compressionof spring [m]

<style>
h1, h2, h3 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>
---
---
### Sim of bow ?!
<br>
<SimIframe 
  src="https://games.crazygames.com/en_US/bowman/index.html"
  height="470px"
/>

<style>
h1, h2, h3 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>


---
---
# Problem Solving
<Problem
  text="John walks down the street and finds out that, what ?!"
  solution="that sims are not working in this presentation"
  imgSrc="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/Free_body1.3.svg/220px-Free_body1.3.svg.png"
/>

---
layout: two-cols
---

<template v-slot:default>

# 3. Friction  Force

Always against motion

</template>
<template v-slot:right>

### Sim of friction ?!
<br>
<Youtube id="A9awBW-Gczk" width="420" height="360"/>

</template>


<style>
h1, h2, h3 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>


---
---
# Sim of friction ?!
<a href="https://ophysics.com/f1.html" target="_blank"> Friction Sim </a>

---
---
# Problem Solving
<Problem
  text="John walks down the street and finds out that, what ?!"
/>
---
---
# Problem Solving
<Problem
  text="John walks down the street and finds out that, what ?!"
  solution="that sims are not working in this presentation"
/>
---
---
# Problem Solving
<Problem
  text="John walks down the street and finds out that, what ?!"
  imgSrc="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/Free_body1.3.svg/220px-Free_body1.3.svg.png"
/>
