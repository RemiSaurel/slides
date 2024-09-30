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

# `memoire`, c'est quoi ?

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
layout: default
transition: slide-left
---
# 🏭 Technos / Architecture

  <div v-click v-motion
  class='absolute'
    :initial="{ x: -100, y: 200 }"
    :enter="{ x: 10, y: 200 }"
  >
    <span class='text-sm font-semibold'> UX/UI  </span>  
    <img src='./assets/figma.svg' width='32'>
  </div>
  <div v-click v-motion
     class='absolute'
    :initial="{ x: -100, y: 300 }"
    :enter="{ x: 10, y: 300 }"
  >
    <span class='text-sm font-semibold'> Gestion projet </span>  
    <img src='./assets/linear.webp' width='48'>
  </div>

  <div v-click v-motion
    :initial="{ x: 180, y: 250 }"
    :enter="{ x: 180, y: 150 }"
  >
    <img src='./assets/archi/local.svg' width='320'>
  </div>
  <div v-click v-motion
    :initial="{ x: -50 }"
    :enter="{ x: 180, y: -290 }"
  >
    <img src='./assets/archi/github.svg' width='300'>
  </div>
  <div v-click v-motion
    :initial="{ x: 600, y: -460 }"
    :enter="{ x: 480, y: -460 }"
  >
    <img src='./assets/archi/dockerhub.svg' width='370'>
  </div>
  <div v-click v-motion
    :initial="{ x: 580, y: -300 }"
    :enter="{ x: 580, y: -460 }"
  >
    <img src='./assets/archi/vps.svg' width='300'>
  </div>

<div class='absolute bottom-2 right-4 text-sm'>
  <SlideCurrentNo />
</div>

<!-- 
Technos récentes mais suffisamment stable pour des projets sur le moyen-long terme mais aussi pour le marché du travail. 
-->
---
layout: default
---
# 🤯 Plusieurs sujets disponibles

<div class='absolute top-3 right-3 text-[#C5C5C5] -rotate-5 '>
  Liste non exhaustive
  <img src='./assets/arrow.svg' width='64' class='-ml-18 -mt-4'  />
</div>

<div class='grid grid-cols-2 gap-4 pt-6'>
  <ProjectCard v-click>
    <template #icon>
      🎮
    </template>
    <template #title>
      <span>Gamification</span>
    </template>
    <template #tags>
      <Tag v-for='tag in ["Design", "Dev", "Archi"]' :key='tag' :content='tag' />
    </template>
    <template #description>
      <span>Basé sur les recommendations de la recherche : ajout de badges, gestion d'amis, expérience de révision, etc.</span>
    </template>
  </ProjectCard>
  <ProjectCard v-click>
    <template #icon>
      🤖
    </template>
    <template #title>
      <span>LLM & création de contenu auto.</span>
    </template>
    <template #tags>
      <Tag v-for='tag in ["IA", "Dev", "Design"]' :key='tag' :content='tag' />
    </template>
    <template #description>
      <span>Utilisation de LLM et IA (<code>Mistral</code>++) pour générer des flashcards (avec un agent ?)</span>
    </template>
  </ProjectCard>
  <ProjectCard v-click>
    <template #icon>
      📱
    </template>
    <template #title>
      <span>Prototype app mobile</span>
    </template>
    <template #tags>
      <Tag v-for='tag in ["Dev", "Design", "Mobile"]' :key='tag' :content='tag' />
    </template>
    <template #description>
      <span>Prototype app mobile : Swift / Kotlin OU React Native, (connexion facile avec le backend / API)</span>
    </template>
  </ProjectCard>
  <ProjectCard v-click>
    <template #icon>
      😄
    </template>
    <template #title>
      <span>Divers</span>
    </template>
    <template #tags>
      <Tag v-for='tag in ["Dev", "Archi", "Design"]' :key='tag' :content='tag' />
    </template>
    <template #description>
      <span>Création de contenu, gestion d'échéances, gestion de l'import, mode collaboratif (multijoueur)</span>
    </template>
  </ProjectCard>
</div>

<div class='absolute bottom-2 right-4 text-sm'>
  <SlideCurrentNo />
</div>

<!-- 
NOTES
-->

---
layout: default
---

# 👋 Merci à tous

N'hésitez pas à venir échanger pour en savoir plus sur le projet !\
\
Discord : @remisaurel\
Mail : saurel@protonmail.com

<div class='absolute bottom-3 left-3 text-[#C5C5C5] rotate-5 '>
  <img src='./assets/arrow.svg' width='64' class='ml-18 mb-2 -rotate-60 transform scale-x-[-1]'  />
  memoire.cloud
</div>

<div class='flex justify-center gap-24 mt-12'>
  <div class='flex flex-col gap-1'>
    🚀 Tester l'app
    <img src='/assets/qr-code.png' width='270'/>
  </div>
  <div class='flex flex-col gap-1'>
    <div class='flex items-center'>✍️ Rejoindre le Discord dédié à <img src='./assets/memoire.png' width='32' /></div>
    <img src='/assets/qr-code-discord.png' width='270'/>
  </div>
</div>