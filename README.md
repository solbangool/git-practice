---
layout: single
title:  "git 사용법 학습"
---

### Mac에서 git 설치하기 

1.  터미널에서 버전 확인   
    ` git --version `

2. Homebrew 설치: https://brew.sh/

3. git 설치<br>
    ` brew install git `

4. 터미널 재실행하여 버전 확인<br>
    ` git --version `

5. source tree 설치
   https://www.sourcetreeapp.com/

6. vs code 설치


---
<br>

### git을 사용하는 2가지 방법
- CLI : 터미널에 명령어 입력해서 사용
- GUI : 소스트리 등의 프로그램 사용

<br>

---
<br>

### 설정 및 프로젝트 관리 방법
1. git 사용자 이름과 이메일 주소를 설정하기<br>
    ` git config --global user.name "(본인 이름)" `

    ` git config --global user.email "(본인 이메일)" `
<br>
   <br>
 - 정상적으로 등록되었는지 확인하기

    ` git config --global user.name `

    ` git config --global user.email `

<br>

2. 관리할 폴더를 git에서 열기
<br>

   > 시작 명령어 

    ` git init `

    > 숨김 파일 보기

    ` command + shift + . `
   
   <br>
    
    * 기본 브랜치명 변경
     
     ` git config --global init.defaultBranch main `
   
   <br>
    

3. 올리지 않아도 되는 파일 관리
   <br>

   > 모든 file.c 

    ` file.c `

    > 최상위 폴더의 file.c

    ` /file.c `

   > 모든 .c 확장자 파일 

    ` *.c `

    > .c 확장자지만 무시하지 않을 파일

    ` !not_ignore_this.c `

   > logs란 이름의 파일 또는 폴더와 그 내용들 

    ` logs `

    > .logs란 이름의 폴더와 그 내용들

    ` logs/ `

   > logs 폴더 바로 안의 debug.log와 .c 파일들 

    ` logs/debug.log `<br>
    ` logs/*.c `
    
    > logs 폴더 바로 안, 또는 그 안의 다른 폴더(들) 안의 debug.log

    ` logs/**/debug.log `

