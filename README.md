# <img src="public/icons/icon_1_96.png" width="45" align="left"> 단어 사전 & 구문 번역 & 저장 크롬 확장 프로그램

### 프로젝트 목적

> 개인 편의를 위한 프로젝트<br/>
> 기존 크롬 확장 프로그램의 manifest 버전 업데이트<br/>
> 평소 어려워하는 영어 구문을 모아서 공부하려는 목적<br/>
> 단순히 Papago API를 이용한 구문 번역이 아닌 LLAMA2를 이용하여 번역시킬 계획<br/>
> Fast API Backend Framework 연동 및 Llama2 모델을 사용하여 다양한 기능 구현 계획<br/>
> 기존 v2 프로젝트 https://github.com/withbbang/chrome-extension

---

### 프로젝트 구조

```
CHROME-EXTENSION-WITH-WEBPACK
├─ config
│  ├─ path.js
│  ├─ webpack.common.js
│  └─ webpack.config.js
├─ public
│  ├─ css
│  │  └─ *.css
│  ├─ icons
│  │  └─ *.png/svg
│  ├─ scripts
│  │  └─ *.js
│  ├─ manifest.json
│  ├─ options.html
│  ├─ popup.html
│  └─ *Offscreen.html
├─ icons
│  └─ *.png/svg
├─ src
│  ├─ background.js
│  └─ *.js
├─ .editorconfig
├─ .gitmessage.txt
├─ .prettierignore
├─ .prettierrc
└─ pack.js
```

---

### 파일 설명

- 📁 config: webpack config 파일들을 담고 있는 디렉터리
- 📁 public: 웹페이지에서 동작하는 파일들을 담고 있는 디렉터리
- > └─ 📄 *Offscreen.html: 크롬 익스텐션이 v3로 업데이트되면서 background.js에서 작업이 가능했던 기능들이 백그라운드에서 동작하도록 환경이 마련됐는데, 해당 html파일과 public/scripts/*Offscreen.js 파일들이 그 부분을 담당한다.
- 📁 src: 코어인 background.js 및 해당 파일에 import 되는 모든 모듈들을 담고 있는 디렉터리

---

### 사용한 API

#### 1) 파파고 네이버 번역 API

- https://openapi.naver.com/v1/papago/n2mt

#### 2) 다음 사전 API

- https://dic.daum.net/search.do?q=word

#### 3) 개인 Fast API Backend Server (계획중)

- Llama2 언어 모델을 이용한 번역 기능 및 추가 기능
- 번역된 구문 DB 저장

---

### 구현화면
