[GitHub repository URL](https://github.com/GimHaLim/MyProject.git)

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

### - 명령어 commit
이 때, **commit**을 이용해서 **git commit -m "(이름)"** 명령을 통해 commit 할 수 있다.

> 현재 상태 : 지금까지의 결과물을 commitmaster-1(이름)로 commit한 상태

</br>

## 3. GitHub 저장소 만들기

이 프로젝트를 GitHub에 올리기 위해서 git status로 현재까지의 상황들이 모두 commit 되어있는지 확인한다.
빠진게 있다면 전부 add해서 commit한다.

### - 명령어 remote
**remote**는 현 폴더의 원격 repository를 확인하는 명령어이다. **git remote**명령으로 확인할 수 있다.

> 현재 상태 : git remote를 입력하면 아직 원격 repository가 없기 때문에 아무것도 나오지 않는다.

[GitHub 사이트](https://github.com/)에 접속을 한다. 계정이 없으면 회원가입을 하고, 로그인을 하면 준비가 끝났다.

GitHub에서 새 Repository를 만들면 GitHub repository의 URL이나 git 명령어가 들어간 여러 정보가 나와있는 page가 뜬다. 여기에서 git remote와 git push가 사용된 명령문을 찾아서 터미널에 복사 붙여넣기를 하면 된다.

> 복사한 내용   
git remote add origin https://github.com/GimHaLim/MyProject.git  
git branch -M main  
git push -u origin main

첫 번째 문장은 GitHub repository를 이 폴더의 origin이란 이름의 원격 저장소로 설정하겠다는 의미이다.

### - 명령어 **push** 
**push**는 원격 저장소에 코드 변경분을 업로드하기 위해서 사용하는 Git 명령어이며, 기본사용법은 **git push origin(저장소 이름) (branch 이름)** 이다.

두 번째 문장은 branch 부분에서 나온다.

세 번째 문장인 **git push -u origin main**은 폴더의 현 branch에 commit된 내용들을 origin의 원격, 즉 이 repository의 main branch에 올리겠다는 의미이다.

> 현재 상태 : GitHub에 새 repository를 만들고 그곳에 remote로 이 프로젝트를 올린 상태.

</br>

## 4. Branch 넘나들기

### - 명령어 **branch**
**branch**는 커밋 사이를 가볍게 이동할 수 있는 어떤 포인터 같은 것이다.   
기본적으로 Git은 master branch를 만든다. 하지만 몇 년 전에 [Black Lives Matter](https://ko.wikipedia.org/wiki/Black_Lives_Matter) 운동에 발맞춰 주종관계를 뜻하는 'master', 'slave'를 다른 단어로 대체하기 위해 repository 생성 시 기본으로 만들어지는 branch 이름을 master에서 main으로 변경하였다. 이것이 앞서 언급했던 두 번째 문장의 이유이다.

**git branch (제목)** 명령을 실행하여 branch를 만들 수 있다.
**git branch**를 입력하면 현재 branch의 종류를 알 수 있다.

### - 명령어 **checkout**
**checkout**을 사용하여 **git checkout (branch 이름)** 명령을 실행하면 branch를 넘나들 수 있다.  
branch 생성과 checkout을 동시에 하려면 **git checkout -b (branch 이름)** 을 한다.

>현재 상태 : 지금까지의 내용을 commit, push하고 새로운 branch인 markdown을 만든 상태

이제 project를 원하는 대로 진행한다.

> 가정 : 4명의 사람이 각각 branch를 통해 Markdown 튜토리얼의 1/4를 맡아서 프로젝트를 진행한다.

> 현재 상태 : 4명이 main에서 branch를 만들어 Markdown 튜토리얼의 조각을 만든 상태. 즉, branch가 main, 위에서 만든 markdown, 각자의 branch 4개로 총 6개인 상태이다.

</br>

## 5. 다른 branch 가져오기

### - 명령어 **merge**
**merge**는 다른 branch에서 일어난 변화를 가져오는 명령어이다.
가져오고 싶은 branch에서 **git merge (변화를 가져올 branch 이름)** 명령을 실행하면 된다.

보통 Hotfix를 해야하는 상황에서 쓰인다.

> 현재 상태 : 지금 현재 4명의 Markdown 튜토리얼 조각들이 흩어져 있으므로 markdown branch에 4개의 branch를 merge하여 그 내용들을 순서대로 markdown branch에 붙여넣었다.