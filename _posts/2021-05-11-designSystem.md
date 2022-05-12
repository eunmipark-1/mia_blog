---
title : "Design System"
category:  planning
tag: large project css planning
toc: true
---
# 큰 프로젝트 투입 시 css planning #

[sample figma file](https://www.frontendmentor.io/challenges/space-tourism-multipage-website-gRWj1URZ3){:target="_blank"}


## 기본 reset ##
[reset css](https://piccalil.li/blog/a-modern-css-reset){:target="_blank"}

## 유틸리티 class ## 

```css
.flex {
  display: flex;
  gap: var(--gap, 1rem);
}

.grid {
  display: grid;
  gap: var(--gap, 1rem);
}

.container {
  padding-inline: 2em;
  margin-inline: auto;
  max-width: 80rem;
}

.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
}

.box {
  background: lightblue;
  padding: 3rem;
}

.call-to-action {
    --gap:5rem;
    background:pink;
    border-radius: 1rem;
}

```

```html
<div class="call-to-action container flex">
    <div class="box">a</div>
    <div class="box">b</div>
    <div class="box">c</div>
    <div class="box">d</div>
</div>
```