#  TIL

------------------------------------

### *CLI*
- **cd** : change directory (ex) cd c:
- **ls** : list segments (현재 작업중인 디렉토리의 폴더 / 파일 
- **mkdir** : make directory
- **' '** : 폴더 생성 시 띄어쓰기 가능
- **touch** : 파일 생성 (touch text.txt, 각 파일 사이에 띄어스기 사용 시 여러개 생성
- **mv** : move (ex. text.txt newfolder -> text.txt파일을 newfolder 폴더로 이동, 오타로 인해 그 이름으로 이동 불가시 이름이 변경 됨
- **rm** : remove (※주의 - 복구 불가)
- **start(mac에선 open)** : 파일 편집기 실행
- **ls -a** : 숨김 파일 나타내기
- **ls -l** : 권한, 생성 시간
- **help** : 도움말 (ex. rm --help)
- **tap** : 폴더/파일 이름 자동완성
- **ctrl + a** : 커서가 맨 앞으로 이동
- **ctrl + e** : 커서가 맨 뒤로 이동
- **ctrl + w** : 커서가 앞 단어를 삭제
- **ctrl + l** : 터미널 화면을 깨끗하게 정리
- **ctrl + insert** : 복사
- **shift + insert** : 붙여넣기

-------------------------------------------------

### *MarkDown : 일반 텍스트 기반의 마크업 언어*

- ```*이탤릭체*```
- ```_이탤릭체2_```
- ```**볼드체1**```
- ```__볼드체2__```
- ```~~취소선~~```
- 인용 : ` (~ 위치에 있음), ```python << 파이썬 언어 인용
- ```[표시할 글자](이동 할 주소) 형태로 작성```
 ```ex) [google](www.google.com)```
- ```![대체 텍스트](이미지 주소) 형태로 작성 ```
 ```ex) ![Git로고](https://git-scm.com/images/logo@2x.png)```
- ```>, >>, >>> : 중첩된 인용문```
- ```------------ : 줄긋기```

-------------------------------------------------

### *git 명령어*

working directory : 로컬의 사용자 작업이 일어나는 곳  
staging area : 커밋을 위한 파일 및 폴더가 추가되는 곳  
repository(commits) : 변경사항(커밋)을 저장하는 곳  

> **커밋 기록자를 등록**
>
> >	git config --global user.name ""
> >	git config --global user.email ""
> >	git config --global -l
>
> **local directory를 git으로 관리**
>
> >	git init 
>
> **git 상태 표시**
>
> >	git status
> >	- untrackted : git이 관리하지 않는 파일
> >	- trackted : git이 관리하는 파일
>
> **staging 단계**
> >	git add 
> >	git add 파일이름(폴더이름)
> >	git add . -> 전체 다
>
> **commit 단계**
> >
> >	git commit -m "메시지"
>
> **commit log 단계**
> >	git log : commit log  
> >	--oneline : 한 줄로 축약해서 보여줍니다.  
> >	--graph : 브랜치와 머지 내역을 그래프로 보여줍니다.  
> >	--all : 현재 브랜치를 포함한 모든 브랜치의 내역을 보여줍니다.  
> >	--reverse : 커밋 내역의 순서를 반대로 보여줍니다. (최신이 가장 아래)  
> >	-p : 파일의 변경 내용도 같이 보여줍니다. (q로 나가기)  
> >	-2 : 원하는 갯수 만큼의 내역을 보여줍니다. (임의의 숫자 사용 가능)  
>
> **원격 저장소 등록**
> >	git remote add <이름> <주소>
> >	  *보통 remote연결이 한 개인 경우 origin을 사용함.
> >	git remote -v => repository 확인
>
> **원격 저장소 삭제**
> >	git remote rm <이름>
> >	git remote remove <이름>
>
> **원격 저장소에 업로드**
>
> >	git push <저장소 이름(origin)><브렌치 이름(master)>