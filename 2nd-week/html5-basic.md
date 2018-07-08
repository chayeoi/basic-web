# HTML5 Basic

## 마크업 요소

상황과 의미에 맞는 적절한 태그의 사용은 사람과 컴퓨터로 하여금 문서의 구조를 더 명확하게 이해할 수 있게 만듭니다. 이번 챕터에서는 앞으로 자주 접하게 될 태그들을 위주로 가볍게 살펴본 후, 이어서 간단한 실습을 진행해보도록 하겠습니다.

### 기본

* `<html>`: html 태그는 모든 HTML 요소의 부모 요소이며 웹 페이지에 단 하나만 존재합니다. html 태그에는 관례적으로 문서의 언어 코드를 알리기 위해 `lang` 속성을 함께 명시합니다. 대표적인 언어코드에는 ko(한국어), en(영어), ja(일본어) 등이 있습니다.

  ```html
  <html lang="ko">
  </html>
  ```

* `<head>`: 문서의 제목, 문자 코드, 키워드 지정, 외부 파일 연결 등 문서의 메타데이터를 기재하기 위한 요소입니다. head 태그 안에 작성한 내용들은 화면에 출력되지 않습니다.
* `<body>`: 문서의 본문 요소로, 실제 화면에 출력되는 HTML 문서의 내용이 body 태그 안에 작성됩니다.

### head

* `<title>`: HTML 문서의 제목을 정의하는 요소로, 검색엔진 최적화(SEO)에도 매우 중요합니다. 정의된 제목은 브라우저 탭에 표시됩니다.

  ```html
  <title>Welcome to Mash-Up!</title>
  ```

* `<meta>`: 문자 코드나 문서의 개요, 키워드 등 브라우저 화면에 나타나지 않는 문서 정보를 기술하는 데 필요한 요소입니다. 주요 meta 요소의 속성은 다음과 같습니다.
  * `charset`: HTML5로 작성된 문서 내에서 문자 코드를 지정하기 위한 속성입니다. 반드시 이 속성 값을 'utf-8'로 지정해줘야 한글이 꺠져보이지 않습니다.
  * `name="description"`: 문서의 개요를 나타내기 위한 속성입니다. 이 속성은 검색엔진에 의해 사용되므로 검색엔진 최적화(SEO)를 위해 중요합니다.
  * `name="keywords"`: 웹 페이지가 검색 엔진에서 어떤 키워드에 노출될지를 지정하기 위한 속성입니다. 검색엔진 최적화(SEO)를 위해 중요합니다.

  ```html
  <meta charset="utf-8">
  <meta name="description" content="Mash-Up 스터디 자료">
  <meta name="keywords" content="Mash-Up, HTML, CSS">
  ```

* `<style>`: CSS를 HTML 문서 내에 직접 기술할 때 사용합니다.

  ```html
  <html>
    <head>
      <style>
        .container {
          background-color: green;
        }
      </style>
    </head>
    <body>
      <div class="container">Mash-Up</div>
    </body>
  </html>
  ```

* `<link>`: 스타일 시트와 같은 외부 리소스를 HTML 문서에 연결할 때 사용합니다.

  ```html
  <html>
    <head>
      <link rel="stylesheet" href="style.css">
    </head>
    <body>
      <div class="container">Mash-Up</div>
    </body>
  </html>
  ```

* `<script>`: HTML 문서에 외부 자바스크립트 파일을 연결하거나 자바스크립트 코드를 직접 기술할 때 사용합니다.

  ```html
  <html>
    <head>
      <script src="index.js"></script>
      <script>
        alert('Hello, HTML!');
      </script>
    </head>
  </html>
  ```

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