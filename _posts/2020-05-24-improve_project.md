---
layout: post
title:  "프로젝트 개선을 위한 방향성"
description: The Fuck 프로젝트 개선을 위한 방향성 제시하기.
date:   2020-05-24 19:03:36 +0530
categories: Python OSS TheFuck Node.js
---

### 지원하지 않는 명령어에 관한 기능 추가 및 개선

#### NVM

 - 저장소 : [`https://github.com/nvm-sh/nvm`](https://github.com/nvm-sh/nvm)

 - NVM 이란?

    NVM은 Node Version Manager로써, Node.js 버전 관리하기 위한 도구입니다.

    OS에 특정 버전의 Node.js를 설치하면, 여러 버전의 Node.js를 사용할 수 없으며, 개발 툴들이 많아짐에 따라 Node.js의 버전을 달리 사용해야 할 필요성이 생겼습니다. 따라서 버전 관리를 위해 NVM 도구가 탄생하게 되었습니다.

 - NVM 명령어들을 지원해야 하는 이유

    Node.js를 주력을 개발하는 개발자의 경우, Node.js를 간편하게 설치할 수 있고, 버전 관리에 용이하기 때문에 NVM 사용은 거의 필수적이라 볼 수 있습니다. 

    따라서 주로 사용되는 명령어에 관련된 기능을 The Fuck에 추가한다면 의미 있는 기여가 될 것이라 생각합니다.

&nbsp;&nbsp;&nbsp;&nbsp;

### 버그 수정

 - [`The Fuck Bug Issue`](https://github.com/nvbn/thefuck/issues?q=is%3Aopen+is%3Aissue+label%3Abug)

   ![The Fuck Bug Issue Image](https://raw.githubusercontent.com/Jokuna/Jokuna.github.io/master/openbug.png)
   
   The Fuck Issue에 등록된 버그 관련 이슈들을 찾고, 이를 해결합니다.

&nbsp;&nbsp;&nbsp;&nbsp;

### 기타

   - the fuck python 기존 코드의 flow에 대한 설명 주석을 추가할 예정

&nbsp;&nbsp;&nbsp;&nbsp;