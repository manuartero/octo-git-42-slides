---
theme: default
layout: cover
background: /images/backgrounds/bg-1.jpg
class: "text-center"
title: cover
highlighter: shiki
lineNumbers: false
colorSchema: 'dark'
info: |
  # Git: Playing With History
  ## A workshop for 42 Campus
# persist drawings in exports and build
drawings:
  enabled: false

fonts:
  sans: "Menlo"
  # use with `font-serif` css class from windicss
  serif: "Robot Slab"
  mono: "Courier"

defaults:
  layout: 'default'
---

# Git: playing with History

@Manuel Artero Anguita

A workshop for 42 Campus

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/manutero/octo-git-42" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
  <a href="https://github.com/manutero/octo-git-42" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <ri:slideshow-line/>
  </a>
</div>

---
layout: intro
image: /images/who-am-i/tetuan-valley.png
title: Who am I?
---

<style>
  .slidev-vclick-hidden {
    display: none;
  }
</style>
# Who am I?

<v-clicks>

- Tetuan Valley (Intern)
- Wayra (Intern)
- Yaap (Junior)
- Doctor 24 (Junior)
- Tuenti (Middle)
- Telefonica (Senior)

</v-clicks>

::right::

<v-clicks>
  <img v-click v-click-hide src='/images/who-am-i/tetuan-valley.png' class="m-40 h-40 rounded shadow" />
  <img v-click v-click-hide src='/images/who-am-i/vuqio.png' class="m-40 h-40 rounded shadow" />
  <img v-click v-click-hide src='/images/who-am-i/yaap.jpeg' class="m-40 h-40 rounded shadow" />
  <img v-click v-click-hide src='/images/who-am-i/doctor24.png' class="m-40 h-40 rounded shadow" />
  <img v-click v-click-hide src='/images/who-am-i/tuenti.png' class="m-40 h-40 rounded shadow" />
  <img v-click v-click-hide src='/images/who-am-i/telefoncia.png' class="m-40 h-40 rounded shadow" />
</v-clicks>

---
layout: section
title: index
---

- One concept

---
layout: statement
background: './public/images/backgrounds/bg-0.jpg'
title: statement I
---

Once you have commit you can't loose your work

---
layout: statement
title: statement II
---

## Once you have commit **you can't losse your work**

---
layout: image
image: /images/main-idea/zelda.png
title: Saving Point
---

commit = saving point

<arrow v-click="1" x1="200" y1="140" x2="300" y2="140" color="#dddddd" width="2" />
<div v-click="2" style="position: absolute;top:120px;left:200px">commit</div>
<arrow v-click="3" x1="200" y1="220" x2="300" y2="220" color="#dddddd" width="2" />
<div v-click="4" style="position: absolute;top:200px;left:200px">commit</div>
<arrow v-click="5" x1="200" y1="300" x2="300" y2="300" color="#dddddd" width="2" />
<div v-click="6" style="position: absolute;top:280px;left:200px">commit</div>

---
layout: center
title: Game run
---

<style>
  .run {
    display: flex;
    flex-direction: column-reverse;
  }
  .branch {
    display: flex;
  }

</style>

<div class="run">
  <openmoji-elf-medium-light-skin-tone v-click="1" class="text-5xl commit green-border" />
  <ph-sword v-click="2" class="text-5xl commit green-border" />
  <div class="branch">
    <bx-book-bookmark v-click="3" class="text-5xl commit green-border" />
    <ph-bird v-click="6" class="text-5xl commit violet-border" />
  </div>
  <div class="branch">
    <la-dragon v-click="4" class="text-5xl commit green-border red" />
    <ph-gift v-click="7" class="text-5xl commit violet-border" />
  </div>
  <div class="branch">
    <dashicons-no v-click="5" class="text-5xl commit green-border red" />
    <la-dragon v-click="8" class="text-5xl commit violet-border red" />
  </div>
</div>

---
layout: two-cols
title: Intro Rebase
---

<style>
  .col-right {
    margin: 0 auto;
  }
  .run {
    display: flex;
    flex-direction: column-reverse;
  }
</style>


# `git rebase`

### Rewrite the history

<br>
<br>

- After getting the sword and the book... <ph-sword class="text-2xl" /> <bx-book-bookmark class="text-2xl" />
- We did beat the bird <ph-bird class="text-2xl" />
- We did get the ~~reward~~ => **SPECIAL REWARD** <ph-gift class="text-2xl gold" />
- We did face the dragon in that conditions
- We did win

::right::

<div class="run">
  <v-clicks>
    <openmoji-elf-medium-light-skin-tone class="text-5xl commit green-border" />
    <ph-sword class="text-5xl commit green-border" />
    <bx-book-bookmark class="text-5xl commit green-border" />
    <ph-bird class="text-5xl commit violet-border" />
    <ph-gift class="text-5xl commit violet-border gold" />
    <la-dragon class="text-5xl commit violet-border" />
    <entypo-trophy class="text-5xl commit violet-border gold" />
  </v-clicks>
</div>

---
layout: cover
background: "/images/backgrounds/bg-1.jpg"
title: Workshop Time
---

asdasd

---

# Foundations: `merge`

`asd`

Slidev is a slides maker and presenter designed for developers, consist of the following features

- 📝 **Text-based** - focus on the content with Markdown, and then style them later
- 🎨 **Themable** - theme can be shared and used with npm packages
- 🧑‍💻 **Developer Friendly** - code highlighting, live coding with autocompletion
- 🤹 **Interactive** - embedding Vue components to enhance your expressions
- 🎥 **Recording** - built-in recording and camera view
- 📤 **Portable** - export into PDF, PNGs, or even a hostable SPA
- 🛠 **Hackable** - anything possible on a webpage

<br>
<br>

Read more about [Why Slidev?](https://sli.dev/guide/why)

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

---

# Navigation

Hover on the bottom-left corner to see the navigation's controls panel, [learn more](https://sli.dev/guide/navigation.html)

### Keyboard Shortcuts

|                                                    |                             |
| -------------------------------------------------- | --------------------------- |
| <kbd>right</kbd> / <kbd>space</kbd>                | next animation or slide     |
| <kbd>left</kbd> / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd>                                      | previous slide              |
| <kbd>down</kbd>                                    | next slide                  |

<!-- https://sli.dev/guide/animations.html#click-animations -->

<img
  v-click
  class="absolute -bottom-9 -left-7 w-80 opacity-50"
  src="https://sli.dev/assets/arrow-bottom-left.svg"
/>

<p v-after class="absolute bottom-23 left-45 opacity-30 transform -rotate-10">Here!</p>

---
layout: image-right
image: /images/repo/create_react_app.png
title: Example repo - main
---

##  <carbon-logo-github /> Octo-Git-42

<br>

- branch: `main`
- commit: `df55345`

<br>

<img src="/images/repo/tree-main.png">

---
layout: image-right
image: /images/repo/replace_favicon.png
title: Example repo - main-layout
---

## <carbon-logo-github /> Octo-Git-42

<br>

- branch: `feat/main-layout`
- commit: `8a134b4`

<br>

<img src="/images/repo/tree-main-layout.png">

---
layout: image-right
image: /images/repo/detects_42.png
title: Example repo - tree-monkey-counter
---

## <carbon-logo-github /> Octo-Git-42

<br>

- branch: `feat/tree-monkey-counter`
- commit: `e7e28c3`

<br>

<img src="/images/repo/tree-monkey-counter.png">

---
layout: image-right
image: /images/repo/fix_and_test.png
title: Example repo - test-monkey-counter
---

## <carbon-logo-github /> Octo-Git-42

<br>

- branch: `test/monkey-counter`
- commit: `c0cb057`

<br>

<img src="/images/repo/tree-test-monkey-counter.png">

---
layout: default
title: resources
---

# Resources

<br><br>

- <a href="https://github.com/manutero/octo-git-42" target="_blank" alt="GitHub"
class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
Repository <carbon-logo-github /></a>

- <a href='https://www.freepik.com/vectors/background' target="_black" alt="Slides"
class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
Slides <clarity-image-gallery-line /></a>

- <a href='https://www.freepik.com/vectors/background' target="_black" alt="Bacground vector"
class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
Free Backgrounds <bi-image /></a>
