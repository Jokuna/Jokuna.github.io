---
layout: post
title:  "프로젝트 소개: The Fuck"
description: 선정한 프로젝트 중 하나인 The Fuck에 대한 설명 및 안내.
date:   2020-05-22 21:03:36 +0530
categories: Python OSS Project
---

[`The Fuck Repository`](https://github.com/nvbn/thefuck)

![texture theme preview](https://raw.githubusercontent.com/nvbn/thefuck/master/example.gif)

The Fuck은 터미널 환경에서 커맨드 입력 오류가 발생했을 경우, fuck 명령어를 통해 이전에 입력한 커맨드 오류를 수정해주고 재입력해주는 툴에 대한 프로젝트 입니다.

명령어 입력 시 오류가 있을 경우 다시 직접 타이핑하는 번거로움이 있지만, The Fuck 툴을 사용하면 번거로움을 줄일 수 있습니다. 

More examples:

```bash
➜ apt-get install vim
E: Could not open lock file /var/lib/dpkg/lock - open (13: Permission denied)
E: Unable to lock the administration directory (/var/lib/dpkg/), are you root?

➜ fuck
sudo apt-get install vim [enter/↑/↓/ctrl+c]
[sudo] password for nvbn:
Reading package lists... Done
...
```

```bash
➜ git brnch
git: 'brnch' is not a git command. See 'git --help'.

Did you mean this?
    branch

➜ fuck
git branch [enter/↑/↓/ctrl+c]
* master
```
&nbsp;&nbsp;&nbsp;&nbsp;

### The Fuck 프로젝트 선정하게 된 이유

초기 프로젝트 선정 시 한국어 형태소를 분석해주는 [`shineware / KOMORAN`](https://github.com/shineware/KOMORAN) , command line fuzzy finder인 [`junegunn / fzf`](https://github.com/junegunn/fzf) , 웹 개발 시 APi 설계, 디자인, 디버깅할때 사용하는  [`Kong / insomnia`](https://github.com/Kong/insomnia) 등등 어떤 프로젝트를 선정할 지에 대해 많은 논의가 진행되었습니다.
 
[`The Algorithm / C`](https://github.com/TheAlgorithms/C) 와 [`The Fuck`](https://github.com/nvbn/thefuck) 가 초기에 선정 되었으나, 최종 프로젝트는 [`The Fuck`](https://github.com/nvbn/thefuck)가 선정이 되었습니다.

[`The Algorithm / C`](https://github.com/TheAlgorithms/C) 프로젝트는 자료구조, 알고리즘 추가하고 간단한 설명 주석으로 달면 쉽게 기여할 수 있지만, [`The Fuck`](https://github.com/nvbn/thefuck) 프로젝트의 경우, 프로젝트의 구조가 직관적이여서 python을 다룰 줄 안다면, 팀원들이 접근하기 쉬우며, 기능 개선과 버그 등 다양한 이슈가 존재하여 알고리즘 프로젝트에 비해 의미 있는 기여를 할 수 있다고 판단하여 선정하였습니다.

&nbsp;&nbsp;&nbsp;&nbsp;

### 설치 가이드

Ubuntu 18.04을 기준으로 작성이 되었습니다.

Ubuntu에서 다음과 같은 명령어를 통해 설치를 진행할 수 있습니다.

```bash
sudo apt update
sudo apt install python3-dev python3-pip python3-setuptools
sudo pip3 install thefuck
```

그 후 `eval "$(thefuck --alias)"` 문구를 `.bashrc` 파일에 작성한 후

```bash
source ~/.bashrc
```
명령어를 치면 바로 사용할 수 있습니다.

&nbsp;&nbsp;&nbsp;&nbsp;

### 최신 버전으로 업데이트

최신 버전으로 업데이트 하기 위해서는 

```bash
pip3 install thefuck --upgrade
```
명령어를 통해 업그레이드를 진행할 수 있습니다.

**참고 문헌 : [`The Fuck installation`](https://github.com/nvbn/thefuck#installation)**

&nbsp;&nbsp;&nbsp;&nbsp;