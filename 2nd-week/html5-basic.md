# HTML5 Basic

## 마크업 요소

지난 시간에도 언급했듯이, 상황과 의미에 맞는 적절한 태그의 사용은 사람과 컴퓨터로 하여금 문서의 구조를 더 명확하게 이해할 수 있게 만듭니다. 이번 챕터에서는 앞으로 자주 접하게 될 태그들을 위주로 가볍게 살펴본 후, 이어서 간단한 실습을 진행해보도록 하겠습니다.

### 기본

* `<html>`
  html 태그는 모든 HTML 요소의 부모 요소이며 웹페이지에 단 하나만 존재합니다.
* `<head>`
* `<body>`

### head

* `<title>`
* `<meta>`
* `<style>`
* `<link>`
* `<script>`

### body

* `<section>`
* `<nav>`
* `<article>`
* `<aside>`
* `<header>`
* `<main>`
* `<footer>`
* `<h1> ~ <h6>`
* `<div>`
* `<p>`
* `<ul>`
* `<ol>`
* `<li>`
* `<dl>`
* `<dt>`
* `<dd>`
* `<figure>`
* `<figcaption>`
* `<blockquote>`
* `<pre>`
* `<a>`
* `<em>`
* `<strong>`
* `<i>`
* `<b>`
* `<small>`
* `<abbr>`
* `<cite>`
* `<q>`
* `<time>`
* `<code>`
* `<sup>`
* `<sub>`
* `<br>`
* `<span>`
* `<del>`
* `<img>`
* `<iframe>`
* `<video>`
* `<audio>`
* `<source>`
* `<canvas>`
* `<table>`
* `<caption>`
* `<thead>`
* `<tbody>`
* `<tfoot>`
* `<tr>`
* `<th>`
* `<td>`
* `<form>`
* `<fieldset>`
* `<legend>`
* `<label>`
* `<input>`
* `<button>`
* `<select>`
* `<optgroup>`
* `<option>`
* `<textarea>`

## 기본적인 마크업 작성 규칙

HTML5는 XHTML 만들어진 표준이므로 존재합니다. 권장되는 방법을 소개하고, 

많이 사용되는 표준

### 종료 태그의 처리

HTML5에서 종료 태그는 생략할 수 있습니다. 즉, `<p><img src="chayeoi.png"></p>`처럼 쓰지 않고 `<p><img src="chayeoi">`로 쓰는 일이 가능합니다. 그러나 이와 같이 종료 태그를 생략할 수 있다고는 하지만, 기존 XHTML 1.0의 규칙처럼 시작과 종료 태그를 정확히 명시하여 정형식(Well-Formed) 구조로 마크업할 것을 권장합니다.

```html
<!-- Ok -->
<p><img src="chayeoi.png">

<!-- Recommended -->
<p><img src="chayeoi"></p>
```

### 대소문자의 사용

시작 태그와 종료 태그는 물론, 속성 이름에 대문자, 소문자를 모두 사용할 수 있습니다. 그러나 기존 XHTML 1.0의 규칙에 따라 소문자만 사용할 것을 권장합니다.

```html
<!-- Ok -->
<IMG src="chayeoi.png" ALT="프로필">

<!-- Recommended -->
<img src="chayeoi.png" alt="프로필">
```

### 빈 요소

'img' 태그와 같이 종료 태그를 갖지 않는 빈 요소들이 있습니다. 기존 HTML4.01에서는 `<img>` 형식으로, XHTML1.0에서는 `<img />` 형식으로 선언해야 하며, HTML5에서는 두 가지 방식을 모두 허용하고 있습니다.

```html
<!-- Ok -->
<img src="chayeoi.png" alt="프로필" />

<!-- Ok -->
<img src="chayeoi.png" alt="프로필">
```

### 속성\(Attribute\)과 값\(Value\)

논리 속성(참 또는 거짓 값만 갖는 속성)의 경우 속성값 지정을 생략할 수 있습니다.

```html
<!-- Ok -->
<select multiple="multiple"></select>

<!-- Recommended -->
<select multiple></select>
```

속성값을 지정할 때 인용 부호를 생략할 수도 있고 홀따옴표 또는 겹따옴표를 사용하여 구분할 수도 있습니다. (개인적으로는 겹따옴표를 사용하여 구분하는 방법을 선호합니다.)

```html
<!-- Ok -->
<img src=chayeoi.png>

<!-- Ok -->
<img src='chayeoi.png'>

<!-- Recommended -->
<img src="chayeoi.png">
```

### 태그의 올바른 중첩 사용

시작 태그와 종료 태그의 중첩에 문제가 발생하지 않도록 주의해야 합니다.

```html
<!-- Never -->
<p>Mash <strong>Up!</p></strong>

<!-- Ok -->
<p>Mash <strong>Up!</strong></p>
```

### 콘텐츠 모델

### HTML 엔티티

HTML 엔티티는 HTML에서 특정 캐릭터들이 예약되어있기 때문에 표기의 혼란을 막기 위해서 사용하는 것입니다. 흔히 공백을 &nbsp; 로 쓰거나 <,>를 &lt; &gt; 처럼 쓰는 것을 말합니다.

https://developer.mozilla.org/ko/docs/Web/HTML
http://html5.clearboth.org/spec
http://html5ref.clearboth.org/