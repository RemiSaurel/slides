---
# You can also start simply with 'default'
theme: default
# some information about your slides (markdown enabled)
title: memoire

drawings:
  persist: false
transition: slide-up
mdc: true
hideInToc: true
---

<div class='text-6xl relative -ml-6 flex items-center gap-2'>
<img src='./assets/memoire.png' width='96' class='mt-2' /> |
memoire
</div>

Présentation M1 Informatique

<img src='./assets/landing.png' width='280' class='absolute right-12 top-6' />
<div class='absolute bottom-4 text-sm'>  Rémi Saurel </div>
<div class='absolute bottom-4 right-16 text-sm'> 13 octobre 2024 </div>

<!--
Bonsoir à tous et merci pour l'invitation.
-->

---
layout: image-right
transition: slide-left
---

# memoire, c'est quoi ?

<ul class='text-xl'>
  <li v-click>🃏 Application web de flashcards</li>
  <li v-click>💻 Open Source</li>
  <li v-click>🔬 Basée sur les résultats de la recherche en EIAH</li>
  <li v-click>😎 Des technos cool </li>
</ul>

<img src='./assets/demo.gif' width='250' class='absolute right-16 top-8' />

<div class='absolute bottom-2 right-4 text-sm'>
  <SlideCurrentNo />
</div>
<!--
NOTES
-->
---
layout: content
transition: slide-left
---
# 🏭 Architecture globale

  <div v-click v-motion
    :initial="{ x: 30, y: 250 }"
    :enter="{ x: 30, y: 150 }"
  >
    <img src='./assets/archi/local.png' width='320'>
  </div>
  <div v-click v-motion
    :initial="{ x: -50 }"
    :enter="{ x: 30, y: -290 }"
  >
    <img src='./assets/archi/github.png' width='300'>
  </div>
  <div v-click v-motion
    :initial="{ x: 900 }"
    :enter="{ x: 330, y: -440 }"
  >
    <img src='./assets/archi/dockerhub.png' width='370'>
  </div>
  <div v-click v-motion
    :initial="{ x: 440, y: -100 }"
    :enter="{ x: 440, y: -445 }"
  >
    <img src='./assets/archi/vps.png' width='300'>
  </div>

<div class='absolute bottom-2 right-4 text-sm'>
  <SlideCurrentNo />
</div>
---
layout: content

---

# 🤖 Technologies

<div class='pt-4 flex flex-col gap-2'>

  <div v-click v-motion
    :initial="{ x: -50 }"
    :enter="{ x: 0 }"
  >
    <span class='text-2xl font-semibold'> 💻 Développement </span>
    <div class='flex items-center gap-8'> 
      <img src='./assets/nuxt.webp' width='162'>
      <img src='./assets/adonis.png' width='162'>
      <img src='./assets/postgresql.png' width='102'>
    </div> 
  </div>

  <div v-click v-motion
    :initial="{ x: -50 }"
    :enter="{ x: 700, y: -160 }"
  >
    <span class='text-2xl font-semibold'> 🎨 UX/UI </span>
    <div class='flex items-center gap-8 py-4'> 
      <img src='./assets/figma.svg' width='34'>
    </div> 
  </div>

  <div v-click v-motion
    :initial="{ x: -50 }"
    :enter="{ x: 0, y: -100 }"
  >
    <span class='text-2xl font-semibold'> ⚙️ Divers </span>
    <div class='flex items-center gap-8'> 
      <img src='./assets/docker.png' width='122'>
      <img src='./assets/github.png' width='122'>
      <img src='./assets/linear.webp' width='122'>
    </div> 
  </div>

</div>

<div class='absolute bottom-2 right-4 text-sm'>
  <SlideCurrentNo />
</div>
---
layout: default
---
# Du coup faut faire quoi ?

### Pleins de choses
Genre ?
### Encore plus

<div class='absolute bottom-2 right-4 text-sm'>
  <SlideCurrentNo />
</div>

---
layout: two-cols
---

# 🚀 Tester `memoire`

<img src='/assets/qr-code.png' width='340'/>

::right::

# 👋 Rejoindre le Discord

<img src='/assets/qr-code-discord.png' width='340'/>

