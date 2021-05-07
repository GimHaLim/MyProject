[GitHub repository URL]()

# Git과 GitHub 사용법 튜토리얼

## 1. Git 저장소 만들기
컴퓨터에서 원하는 위치에 프로젝트를 진행할 폴더를 만들고 이 폴더를 VS Code로 연다.  
폴더 안에 프로젝트에 들어갈 파일을 만들고 저장한다.  

> 현재 상태 : MyProject 폴더를 바탕화면에 만들고 VS Code로 열어서 README.md 파일을 만듦.  

**ctrl + `** 를 눌러 하단에 터미널을 열고 Git 명령을 실행하면 된다.

### - 명령어 init

**init**을 사용해서 **git init** 명령을 실행하면 빈 저장소가 만들어졌다는 메시지가 뜬다. 이 폴더가 Git의 관리 하에 들어간 것이다.

### - 명령어 config

**config**를 사용해서 다음과 같이 사용자 정보를 등록한다.

- git config --global user.name "(내 이름)"
- git config --global user.email "(내 메일 주소)"

> 현재 상태 : 터미널을 열어 명령어(init, config)를 통해 폴더가 Git의 관리를 받게 하고, Git에 사용자 정보를 등록한 상태. 

</br>

## 2. 현재 시점을 저장하기

우선 지금까지 했던 것을 저장한다! 이 점을 꼭 지켜야 한다.

### - 명령어 status

**status**를 사용해서 **git status** 명령을 실행하면 현재 상태를 알 수 있다.   
예를 들어, 내용이 수정되었거나 파일이 추가된 경우가 있다.

> 현재 상태 : README 파일은 새로 만든 파일이기 때문에 git status를 실행하면 'Untracked files'에 들어 있다. 아직 commit에 넣어지지 않은 파일이라는 뜻이다.

### - 명령어 add

**add**를 사용해서 **git add -A** 명령을 실행하면 파일을 새로 추적할 수 있다.  
다시 **git status**를 하면 commit할 수 있는 목록이 나온다.
