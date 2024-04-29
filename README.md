
# :hatched_chick::hatched_chick::hatched_chick: **Git 용어정리** :hatched_chick::hatched_chick::hatched_chick:

### :seedling: **git config**

  1-1) git config에 있는 모든 setting 출력

      $ git config --list

  1-2).gitconfig 파일 열기
  
      $ git config --global -e

  1-3) 기본 에디터 설정
  
      $ git config --global core.editor 'code --wait'

  1-4) 사용자 정보 등록
  
      $ git config --global user.name  # 'name'
      $ git config --global user.email # 'email'
      
      $ git config user.name           # 'user name 확인'
      $ git config user.email          # 'user email 확인'

  1-5) Auto CRLF 설정
  
      $ git config --global core.autocrlf true  # Windows 환경
      $ git config --global core.autocrlf input # MAC 환경

--------

### :seedling: **Git init & add**

  1-1) git 초기화

      $ git init
  
  1-2) git add
      
      $ git add a.txt        # a.txt 라는 파일 stage
      $ git add a.txt b.txt  # a.txt, b.txt 라는 파일 stage
      $ git add *.txt        # .txt로 끝나는 모든 파일 stage
      $ git add *            # 삭제된 파일 & .으로 시작하는 파일 제외 모든 파일 stage
      $ git add .            # 모든 파일 stage

--------

### :seedling: **Git commit**
  
      $ git commit
      $ git commit -m 'Commit message' 
      $ git commit -am 'Commit message'   # 수정된 파일에 add와 커밋 동시에 하기 
--------

### :seedling: **Git log**

      $ git log
      $ git log --patch                   # 커밋 별로 발생한 차이 출력
      $ git log --oneline                 # 커밋 당 한줄로 출력
      $ git log --oneline --reverse       # 한 줄로 출력, 과거 > 현재 
--------

 ### :seedling: **Git remote**

#### **원격 저장소 URL 출력**
      $ git remote -v 

      # example 
      $ git remote -v
      origin https://github.com/Dabin/Dabin.github.io.git (fetch)
      origin https://github.com/Dabin/Dabin.github.io.git (push) 

#### **로컬 저장소에 원격 저장소 주소 알려주기**
      git remote add name URL

      # example
      $ git remote add origin http://github.com/Dabin/feature-eda.git
--------

 ### :seedling: **Git push**

#### **원격 저장소에 커밋 push하기**
       $ git push origin master 
      
#### **지정 태그 push하기**      
       $ git push origin --tags

#### **모든 태그 push하기**
       $ git pysh origin --tags

#### **원격 저장소에 있는 태그 삭제하기**
       $ git push origin --delete v1.2.3

--------

 ### :round_pushpin:**git branching diagram**
<br>
<img src="https://github.com/DabinNovelis/How-to-use-the-git-git-/assets/155599008/68d6a379-e2ae-4a9e-9ffc-fe5ea1a37391" width="800" />
       
