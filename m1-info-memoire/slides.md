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
layout: default
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
<!-- 
Technos récentes mais suffisamment stable pour des projets sur le moyen-long terme mais aussi pour le marché du travail. 
-->
---
layout: default
---
# 🤯 Plusieurs sujets disponibles

<div class='grid grid-cols-2 gap-4 pt-6'>
  <ProjectCard v-click>
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
    <template #title>
      <span>Prototype app mobile</span>
    </template>
    <template #tags>
      <Tag v-for='tag in ["Dev", "Design", "Mobile"]' :key='tag' :content='tag' />
    </template>
    <template #description>
      <span>Prototype app mobile : Swift / Kotlin OU React Native, développement <span class='italic'>isolé</span> (API facilement utilisable)</span>
    </template>
  </ProjectCard>
  <ProjectCard v-click>
    <template #title>
      <span>Divers</span>
    </template>
    <template #tags>
      <Tag v-for='tag in ["Dev", "Archi", "Design"]' :key='tag' :content='tag' />
    </template>
    <template #description>
      <span>Création de contenu, Gestion d'échéances, Gestion de l'import, Mode collaboratif (multijoueur)</span>
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
Discord : @remisaurel

<div class='flex justify-center gap-24 mt-12'>
  <div class='flex flex-col gap-1'>
    🚀 Tester l'app
    <img src='/assets/qr-code.png' width='270'/>
  </div>
  <div class='flex flex-col gap-1'>
    ✍️ Rejoindre le Discord
    <img src='/assets/qr-code-discord.png' width='270'/>
  </div>
</div>