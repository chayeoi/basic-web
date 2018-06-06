# 실습 환경 구성하기

본격적인 학습을 시작하기에 앞서, 웹 프론트엔드 개발에 필요한 최소한의 실습 환경을 함께 구성해보겠습니다.

## 텍스트 에디터: Visual Studio Code

소프트웨어를 개발하기 위해서는, 우리가 원하는 작업을 올바르게 수행하도록 컴퓨터에게 적절한 명령을 내릴 수 있어야 합니다. 그러나 컴퓨터는 우리가 일상에서 사용하고 있는 자연어를 이해하지 못하기 때문에 **사람과 컴퓨터가 모두 이해하고 소통할 수 있는 중간 매개체가 필요**한데, 그 매개체 역할을 하는 것이 바로 프로그래밍 언어입니다. 우리는 이것을 통해 컴퓨터에게 특정한 작업을 수행하도록 명령을 내릴 수 있습니다.

우리가 앞으로 학습하게 될 웹을 예로 들어보겠습니다. 보통의 경우, 하나의 웹 페이지를 구성하기 위해서 기본적으로 HTML과 CSS, 그리고 Javascript라는 세 종류의 언어를 사용합니다. 각 언어를 사용하여 우리는 .html, .css, .js 확장자를 갖는 파일을 작성하게 되는데, 이러한 파일들을 편집하기 위해서는 **텍스트 에디터**라는 특별한 도구가 필요합니다.

일반인들에게 가장 친숙한 텍스트 에디터로 윈도우의 메모장, 맥의 텍스트 편집기가 있습니다. 이들 에디터를 사용하더라도 앞서 언급했던 확장자를 갖는 파일을 작성하는 것이 가능하지만, 코드를 편집하는 일에 특화된 에디터가 아니기 때문에 개발을 할 때는 그리 유용하지 않습니다. 대신, 지금 소개 Visual Sutdio Code를 사용하게 되면 코드 자동 완성, 문법 오류 검출 등 기타 유용한 확장 기능의 도움을 받으면서 개발 생산성을 크 향상시킬 수 있습니다.

### Visual Studio Code

Visual Studio Code는 마이크로소프트에서 개발한 텍스트 에디터로, 개발에 편리한 각종 기능들을 제공합니다. 아래 링크를 통해 VSCode를 다운로드할 수 있습니다.

[Visual Studio Code 다운로드](https://code.visualstudio.com/docs/?dv=osx)

### Extension 설치

VSCode 마켓 플레이스에 들어가면 개발에 유용한 다양한 익스텐션들을 설치할 수 있습니다.

* Emmet: 매우 간단한 몇 가지 코드만 입력하면, 자동으로 완전한 HTML 코드를 생성해 주는 유용한 플러그인입니다. VSCode에 기본적으로 내장되어 있기 때문에 따로 설치하지 않아도 됩니다.
* Auto Close Tag: 오프닝 태그만 입력하면 자동으로 알아서 클로징 태그를 완성해주는 플러그인입니다.
* Auto Rename Tag: HTML 파일 내에서 이미 작성된 태그의 종류를 변경해야 할 때, 오프닝 태그와 클로징 태그 중 한 쪽만 수정해도 그에 대응하는 반대쪽 태그도 함께 수정시켜주는 플러그인입니다.
* Guides: Guides는 들여쓰기\(Indentation\) 깊이의 정도를 시각적으로 파악하기 쉽게 해줍니다.
* IntelliSense for CSS class names in HTML: HTML 파일의 `style` 태그 안에서 직접 선언되었거나 `link` 태그를 통해 연결된 외부 스타일 시트에 선언된 클래스명에 대하여, 몇 글자만 입력하면 자동 완성된 클래스명을 제안해주는 플러그인입니다.
* Live Server: Live Reload 기능이 포함된 로컬 서버를 실행하여 코드를 수정 후 저장할 때마다 자동으로 변경된 이력이 반영된 새 페이지를 로드해줍니다.
* Prettier: 우리가 작성한 코드가 항상 일관된 스타일을 유지할 수 있도록 들여쓰기 등 포맷과 관련된 부분을 이쁘게 정리해주는 매우 유용한 플러그인입니다.

## 웹 브라우저: Chrome, Firefox

동일한 웹 페이지라고 하더라도, 사용자가 이용하고 있는 브라우저의 종류에 따라 보여지는 결과물에는 조금 씩 차이가 있을 수 있습니다. 이는 **각 브라우저 별로 기본값으로 적용하고 있는 스타일\(User Agent Style Sheet\)도 다를 뿐더러, 특정 브라우저에서는 지원되지 않는 스타일 속성들이 존재하기 때문**인데요. 이런 이유로 인해 개발자는 사용자가 브라우저의 종류에 얽매이지 않고 항상 동일한 결과물을 받아볼 수 있도록 노력해야 합니다. 이 수업에서 우리는 Chrome과 Firefox 두 종류의 브라우저를 사용하여 우리가 작업한 결과물을 확인하도록 하겠습니다.

### Chrome

아래 링크로 이동해 Chrome 설치 파일을 다운로드합니다.

[Chrome 다운로드](https://www.google.co.kr/chrome/index.html)

Chrome 브라우저를 설치를 완료하셨다면, 개발에 유용한 몇 가지 확장 도구들을 더 설치해보도록 하겠습니다.

* [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm?hl=ko): CSS 스타일 속성 제거, 스크립트 제거 등 각종 요소를 비활성시킬 수 있는 기능을 제공하여 다양한 환경에 대한 테스트를 진행하거나, 화면 상의 픽셀을 측정할 수 있는 Ruler를 제공하는 등 웹 프론트엔드 개발에 도움이 될 만한 다양한 기능을 내장하고 있습니다.
* [headingsMap](https://chrome.google.com/webstore/detail/headingsmap/flbjommegcjonpdmenkdiocclhjacmbi?hl=ko): Heading의 구조에 따른 문서의 개요\(Outline\)를 추출해줍니다.
* [OpenWAX](https://chrome.google.com/webstore/detail/openwax/bfahpbmaknaeohgdklfbobogpdngngoe?hl=ko): 웹 접근성 관련 문제를 진단하기 위한 가이드라인을 제공해주는 툴입니다.

### Firefox

아래 링크로 이동해 Firefox 설치 파일을 다운로드합니다.

[Firefox 다운로드](https://github.com/chayeoi/basic-web/tree/b6ba30fdbaeb0a86bf5430277c245f5fbfcbce7b/1/[https:/www.mozilla.org/ko/firefox/new/README.md)

Chrome 브라우저에 설치했던 Web Developer 툴을 Firefox에도 설치하겠습니다.

* [Web Developer](https://addons.mozilla.org/ko/firefox/addon/web-developer/?src=search)

## 버전 관리 시스템: Git

혹시, 아래와 같은 상황을 겪어보진 안았나요?

1. 내가 작업한 결과물의 다양한 버전을 만들기 위해 여러 개의 사본을 생성\(예시: 메인 칼라를 '빨강'에서 '파랑'으로 변경\)
2. 최종 시안으로 생각했던 작업물이 클라이언트나 팀원의 요구에 따라 조금씩 변경될 때마다 '다른 이름으로 저장'하면서 최종이라고 이름 지어진 여러 개의 파일을 생성\(`'최종.psd', '최종 final.psd`, '진짜 최종.psd'...\`\)

매번 이러한 상황에 처했다면 Git을 배울 차례입니다.

버전 관리 시스템이란 **파일의 변화를 시간에 따라 기록하여 과거 특정 시점의 버전을 다시 불러올 수 있는 시스템**을 일컫습니다.\(출처: Git 공식 문서\) Git은 이러한 버전 관리 시스템 중의 하나로, 빠른 속도와 Git의 가장 큰 특징 중 하나인 분산 모델이 갖는 수많은 장점으로 인해 개발자 사이에서 압도적인 점유율로 사용되어지고 있습니다.

Git이 어떤 일을 하는지 대략적인 감을 잡으셨다면, 지금부터는 Git을 설치하고 기본적인 사용법을 익혀보겠습니다.

### Git 설치하기

macOS에서 Git을 설치하는 대표적인 2가지 방법을 소개하겠습니다.

#### Git 공식 사이트에서 설치 파일을 다운로드

[Git 공식 사이트](https://git-scm.com/download/mac)로 이동하여 설치 파일을 다운로드할 수 있습니다. 다운로드가 완료되면 해당 파일을 실행하여 안내하는 절차를 따라 설치를 완료합니다.

#### Xcode를 통해 설치하기

Xcode는 애플이 만든 운영체제에서 동작하는 소프트웨어를 개발하기 위한 통합 개발환경\(IDE, Intergrated Development Environment\)입니다. Xcode를 설치하게 되면 기본적으로 '명령어 라인 도구\(Command Line Tools\)'가 함께 설치되고 명령어 라인 도구에는 Git을 비롯한 다양한 UNIX 스타일 명령어 툴들이 포함되어 있기 때문에, Xcode 설치 한 번으로 Git도 함께 설치가 됩니다. Xcode는 Mac 앱 스토어에 접속하여 설치할 수 있습니다.

고작 '명령어 라인 도구'를 설치하고자 꽤나 큰 용량을 차지하는 Xcode를 설치하는 일이 비효율적으로 느껴질 수도 있습니다. 특별히 Xcode를 사용할 일이 없다면, '명령어 라인 도구'만 따로 내려받는 것 역시 가능합니다. 터미널을 실행 후 다음 명령을 입력하면 됩니다. 터미널\(Ternminal\)은 GUI 위에서 동작하는 커맨드 라인 인터페이스\(CLI\)로, 맥 OS에 기본적으로 설치되어있습니다.\(출처: 나무위키\)\)

{% code-tabs %}
{% code-tabs-item title="Git 설치" %}
```bash
xcode-select --install
```
{% endcode-tabs-item %}
{% endcode-tabs %}

```text
xcode-select --install
```

### Git 기본

커맨드 라인으로 git을 사용할 수도 있지만, VSCode는 에디터 차원에서 Git과 통합하여 버전 관리 기능을 제공.

```bash
git init
git add
git commit
git push
git pull
```

```bash
cd
mkdir
```

지금까지 프론트엔드 개발에 필요한 최소한의 실습 환경을 함께 구성해보았습니다. 필요할 때가 되면 설치하도록 하겠습니다.

