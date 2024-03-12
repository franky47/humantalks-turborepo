---
# try also 'default' to start simple
theme: default
defaults:
  layout: center
  transition: none
title: Economisez votre CI avec Turborepo
class: text-center
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
# transition: fade
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
mdc: true
layout: cover
transition: fade
---

# Economisez votre CI avec **Turborepo**

Comment gagner des **années** de temps de CI en quelques **minutes**.

---
title: About:me
---

# **François Best**

https://francoisbest.com

Développeur web freelance

Contributeur open-source

---
layout: section
---

# **C'est quoi un monorepo ?**

---
layout: image-right
image: /nuqs-files.png
transition: fade
---

<h1 class="text-6xl font-bold">Monorepo<span class="text-gray-500">sitory</span></h1>

<ul class="text-xl">
  <li v-click>Plusieurs projets (liés ou non)</li>
  <li v-click>Un seul repository / dépôt de code</li>
  <li v-click>Un seul historique Git</li>
  <li v-click>Un seul CI / CD pour l'ensemble</li>
  <li v-click>Plusieurs équipes</li>
</ul>

---
layout: image
image: /sauron.jpg
transition: fade
---

<h1 class="font-bold text-shadow-xl text-center">Une CI pour les gouverner tous</h1>

---
layout: section
---

# Problème: la **redondance**.

<img alt="C'est pas faux" src="/perceval.gif" class="mx-auto block"/>

<!-- On perd du temps à refaire les même choses, pas nécessaire -->

---
layout: cover
---

# **Solutions**

<ol class="text-3xl space-y-8">
<li v-click>

**Éviter** de faire du travail inutile <span class="text-gray-500">(cache)</span>

</li>
<li v-click>

**Paralléliser** le reste autant que possible

</li>
</ol>

---

<h1 style="font-size:4rem;">Turborepo n'est <strong>pas</strong>:</h1>

<ul class="text-3xl space-y-8 my-16">
<li v-click>

Un gestionnaire de _dépendences_ <span class="text-gray-500">(npm, yarn, pnpm)</span>

</li>
<li v-click>

Un gestionnaire de _workspace_ <span class="text-gray-500">(built-in, lerna)</span>

</li>
</ul>

<v-click>

<p class="text-3xl">C'est un gestionnaire de <em><strong>tâches</strong></em>.</p>

</v-click>


<!--

3. Scripts dans package.json (build, test, lint)
-->

---

<h1 style="font-size:4rem;">Le cache</h1>

<ul class="text-3xl space-y-2 my-16">
  <li v-click>Entrées: sources & environnement</li>
  <li v-click>Sorties: artéfacts & logs</li>
  <li v-click>Hashing</li>
  <li v-click>Distribution</li>
</ul>

---
layout: image
image: /cache-miss.webp
backgroundSize: contain
---

# Cache **MISS**

---
layout: image
image: /cache-hit.webp
backgroundSize: contain
---

# Cache **HIT**

---
layout: image-left
image: /remote-cache.png
backgroundSize: contain
---

<!-- Le superpouvoir de Turborepo: le cache distribué -->

# Cache **distribué**

- Accélération des équipes
- Parallélisation du CI (matrices)

---

# Alternatives

<p/>

<svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="h-24 w-24" fill="currentColor"><title>Nx</title><path d="m12 14.1-3.1 5-5.2-8.5v8.9H0v-15h3.7l5.2 8.9v-4l3 4.7zm.6-5.7V4.5H8.9v3.9h3.7zm5.6 4.1a2 2 0 0 0-2 1.3 2 2 0 0 1 2.4-.7c.4.2 1 .4 1.3.3a2.1 2.1 0 0 0-1.7-.9zm3.4 1c-.4 0-.8-.2-1.1-.6l-.2-.3a2.1 2.1 0 0 0-.5-.6 2 2 0 0 0-1.2-.3 2.5 2.5 0 0 0-2.3 1.5 2.3 2.3 0 0 1 4 .4.8.8 0 0 0 .9.3c.5 0 .4.4 1.2.5v-.1c0-.4-.3-.5-.8-.7zm2 1.3a.7.7 0 0 0 .4-.6c0-3-2.4-5.5-5.4-5.5a5.4 5.4 0 0 0-4.5 2.4l-1.5-2.4H8.9l3.5 5.4L9 19.5h3.6L14 17l1.6 2.4h3.5l-3.1-5a.7.7 0 0 1 0-.3 2.7 2.7 0 0 1 2.6-2.7c1.5 0 1.7.9 2 1.3.7.8 2 .5 2 1.5a.7.7 0 0 0 1 .6zm.4.2c-.2.3-.6.3-.8.6-.1.3.1.4.1.4s.4.2.6-.3V15z"></path></svg>

<img src="/rush.svg" style="filter:invert(100%) hue-rotate(180deg);"/>

---
layout: cover
---

# Démo & Questions

Merci à Raise Partner pour l'accueil !
