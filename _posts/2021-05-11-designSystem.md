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


.box {
  background: lightblue;
  padding: 3rem;
}

.call-to-action {
    --gap:5rem;
    background:pink;
    border-radius: 1rem;
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

```

```html
<div class="call-to-action container flex">
    <div class="box">a</div>
    <div class="box">b</div>
    <div class="box">c</div>
    <div class="box">d</div>
</div>
```

--gap 값이 상속되어 간격이 넓어짐을 확인할 수 있다.

.sr-only :  시각적으로 사라지나 DOM 흐름에서는 존재하므로 스크린 리더를 통해서는 접근 할 수 있다. 


## color utility class ##  

hsl : 알파값 핸들링하기가 편리하다.  ex: hsl (230 35% 7% / .5)

```css
/* ------------------------ */
/* Custom properties        */
/* ------------------------ */

:root {
   --clr-dark: 20 35% 7% ;
   --clr-light: 231 77% 90%;
   --clr-white: 0 0% 100%; 
}

.bg-dark { background-color: hsl( var(--clr-dark) );}
.bg-accent { background-color: hsl( var(--clr-light) );}
.bg-white { background-color: hsl( var(--clr-white) );}

.text-dark { color: hsl( var(--clr-dark) );}
.text-accent { color: hsl( var(--clr-light) );}
.text-white { color: hsl( var(--clr-white) );}

.example-component {
    background-color:hsl( var(--clr-light) / .2);    
}
```

```html
<div class="container">
    <h1>Design system</h1>
    <div class="bg-accent text-dark" style="padding:1rem;">light blue bg, with dark text</div>
    <div class="bg-white text-dark" style="padding:1rem;">white bg, with dark text</div>
    <div class="example-component text-white" style="padding:1rem;">light blue bg, with a 20% alpha and white text</div>
</div>
```


## Typography part ##


## numbered Title ##  


## interacitve elements ## 



## underline indicators ## 