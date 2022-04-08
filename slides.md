---
theme: default
layout: cover
background: /images/backgrounds/bg-1.jpg
class: "text-center"
title: Cover
highlighter: shiki
lineNumbers: false
colorSchema: "dark"
info: |
  # Git: Playing With History
  ## A workshop for 42 Campus
hideInToc: true

# persist drawings in exports and build
drawings:
  enabled: false

fonts:
  sans: "Menlo"
  # use with `font-serif` css class from windicss
  serif: "Robot Slab"
  mono: "Courier"
---

# Git: playing with History

@Manuel Artero Anguita

A workshop for 42 Campus

---
layout: intro
title: Who am I?
hideInToc: true
---

<style>
  span {
    color: pink;
  }
</style>

# Who am I?

<v-clicks>

- Tetuan Valley (Intern) <span>[ 2012 ]</span>
- Wayra (Intern) <span>[ 2013 ]</span>
- Yaap (Junior) <span>[ 2014 ]</span>
- Doctor 24 (Junior) <span>[ 2015 ]</span>
- Tuenti (Middle)<span>[ 2017 ]</span>
- Telefonica (Senior)<span>[ 2022 ]</span>

</v-clicks>

---
layout: section
title: index
hideInToc: true
---

<Toc />

---
layout: statement
title: Statement
---

Once you `$> git commit`, you can't loose your work.

---
layout: statement
title: Statement II
hideInToc: true
---

## Once you `$> git commit`,

## **you can't losse your work**

---
layout: image
image: /images/main-idea/zelda.png
title: Saving Points
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
hideInToc: true
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
layout: two-cols
title: In a Nutshell
---

### Before

<br>

```bash
$(my-branch)> git status
```

```

A---B---C---F---G (main)
         \
          D---E (HEAD my-branch)

```

::right::

### After

<br>

```bash
$(my-branch)> git rebase main
```

```
 A---B---C---F---G (main)
                  \
                   D'---E' (HEAD my-branch)

```

---
layout: cover
background: "/images/backgrounds/bg-1.jpg"
title: Workshop Time
---

## Show me the code

---
layout: image-right
image: /images/repo/create_react_app.png
title: Example repo - main
hideInToc: true
---

## <carbon-logo-github /> Octo-Git-42

- branch: `main`
- commit: `df55345`

<br>

<img src="/images/repo/tree-main.png">

---
layout: image-right
image: /images/repo/replace_favicon.png
title: Example repo - main-layout
hideInToc: true
---

## <carbon-logo-github /> Octo-Git-42

- branch: `feat/main-layout`
- commit: `8a134b4`

<br>

<img src="/images/repo/tree-main-layout.png">

---

layout: image-right
image: /images/repo/detects_42.png
title: Example repo - tree-monkey-counter
hideInToc: true

---

## <carbon-logo-github /> Octo-Git-42

- branch: `feat/tree-monkey-counter`
- commit: `e7e28c3`

<br>

<img src="/images/repo/tree-monkey-counter.png">

---
layout: image-right
image: /images/repo/fix_and_test.png
title: Example repo - test-monkey-counter
hideInToc: true
---

## <carbon-logo-github /> Octo-Git-42

- branch: `test/monkey-counter`
- commit: `c0cb057`

<br>

<img src="/images/repo/tree-test-monkey-counter.png">

---
layout: center
title: Cheat Sheet
---

## git rebase `--interactive`

```bash

# Commands:
# p, pick <commit> = use commit
# r, reword <commit> = use commit, but edit the commit message
# e, edit <commit> = use commit, but stop for amending
# s, squash <commit> = use commit, but meld into previous commit
# f, fixup <commit> = like "squash" but keep only the previous commit's log message.
# x, exec <command> = run command (the rest of the line) using shell
# b, break = stop here (continue rebase later with 'git rebase --continue')
# d, drop <commit> = remove commit

```

---
layout: image
image: /images/dr-strange.jpg
title: Responsibility
---

## With great power comes...

<br>

- public branches
- `merge` vs. `rebase`
- ~~`pull --force`~~ `reset --hard`

---
layout: default
title: Internals
---

## Internals

<br>

```c {all|4,5,7,8|2,3,10,11}
struct Commit {
  uuid_t sha;
  Commit parent;
  char msg[];
  Blob content[];

  User author;
  time_t timestamp;

  User commiter;
  time_t commit_timestamp;

  ...
};
```

---
layout: two-cols
title: onto
hideInToc: true
---

### Before

```bash
git rebase `--onto <new-base> <old-base>`
```

```

Before
A---B---C---F---G (main)
         \
          D---E---H---I (HEAD my-feature)

```

::right::

### After

```
git rebase --onto F D
```

```

A---B---C---F---G (main)
             \
              E'---H'---I' (HEAD my-feature)

```

---
layout: center
title: Form
---

<style>
  h1 svg {
    width: 400px;
    height: 400px;
  };

  h1 svg:hover {
    color: gold;
  };
</style>

<h1>
  <a href="https://forms.gle/s4upYsGyzY2UEu7J6">
    <carbon-location-star />
  </a>
</h1>

---
layout: default
title: Resources
hideInToc: true
---

# Resources

<br>

- <a href="https://github.com/manutero/octo-git-42" target="_blank" alt="GitHub"
  class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
  Repository <carbon-logo-github /></a>

- <a href='https://github.com/manutero/octo-git-42-slides/blob/main/slides-export.pdf' target="_black" alt="Slides"
  class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
  Slides <clarity-image-gallery-line /></a>

- <a href='https://www.freepik.com/vectors/background' target="_black" alt="Bacground vector"
  class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
  Free Backgrounds <bi-image /></a>

---
layout: image
image: /images/spiderman-42.jpg
title: End
hideInToc: true
---

# OK?
