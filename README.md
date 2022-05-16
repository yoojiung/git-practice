# Git

## 첫설정
개행문자(new line) 설정
```
$git config --global core.autocrlf input
```

## 사용자 정보

```
$git config --global user.name"abc"
$git config --global user.email "abc@abc.com"
```

## 구성확인
```
$git config --global --list
```
***
## 프로젝트에서 추적시작
```
$git init
```

## 특정파일만 추적
```
$ git add 파일명
```

## 깃허브에 필요없는 파일 빼기
1.gitignore 파일 만들기  

2.gitignore에 파일 혹은 폴더 이름 집어넣기

## 모든 파일의 변경사항을 추적하도록 지정 
```
$git add .
```

## 수정사항 확인
```
$ git status
```

## 메세지와 함께 버전을 생성
```
$git commit -m "message"
```

## 원격 저장소로 연결
```
$git remote add origin 저장소 주소
```

## 현재 지정된 원격주소 삭제
```
$git remote remove origin
```

## 원격 저장소로 버전 내역 전송
```
$git push origin master
```

## 저장된 커밋내용 확인
```
$git log
```

## 깃폴더 삭제
setting에서 danger zone 에서 삭제 가능

## 이전버전돌아가기
```
$git reset --hard HEAD~n
```

## 이전 버전 돌아 간 것 되돌리기
```
$git origin --hard ORIG_HEAD
```


***
## git branch
branch란  master라는 곧은가지가 있는데 예를 들면 그 페이지에 로그인 페이지를 
개발을 할려고 하면 master에 영향이 가지 않게 개발을 할 수 있도록 하는 것
로그인 페이지가 개발이 끝나면 merge(병합)을 통해 master로 연결한다

## 브랜치 목록 확인
```
$git branch
```

## 브랜치 추가
```
$git branch abc
```

## 브랜치 변경
```
$git checkout abc
```

## pull requests (병합 merge)
master가 아닌 다른 branch로 작업이 완료가 되고 commit이 되면
git으로 들어가서 브랜치에 잘 있나 확인하고 메뉴 2번째에 있는 pull requests를
눌러 병합을 할 수 있다 

## 주의
>다른 브랜치로 원격 저장소에 push할 때  
>git push origin branch이름 확인 잘 할 것!
***
## git clone
깃허브에 저장된 코드들을 가져와서 작업할 수 있다

### 사용법 :
1.Repositories에서 프로젝트 코드 주소 복사  
2.vscode 터미널에서 맥은 ls 윈도우는 dir을 눌러 시작할 곳을 찾는다  
3.cd desktab  
4.주소 붙여넣기

## clone에서 가져온 프로젝트 branch 목록 확인하기
```
$git branch -r
```

## 클론해서 가져온 프로젝트를 다른 branch로 쓰는 법
```
$git checkout -t branchname
```

## clone에서 가져온 프로젝트 branch 삭제
```
$git branch -d abc
```

## clone에서 가져온 프로젝트 branch 생성과 동시에 접속
```
$git checkout -b abc
```













