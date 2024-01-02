# command

## 리눅스 명령어
`pwd` 현재 위치 경로 보기

`ls` 디렉터리 보기 (/는 디렉터리)

`ls -l` 상세 정보 포함 디렉터리 보기

`clear` 화면 초기화

`cd ..` 상위 디렉토리

`cd " "` 디렉토리 이동

`cd ~` 홈 디렉토리 이동

`mkdir " "` 디렉토리 생성

`rm -r " "` 디렉토리 제거(-r 하위 디렉토리까지 제거)

`exit` 터미널 종료

`cat " "` 텍스트 파일 내용 보기

`cat "A"s > "B"` A를 연결해서 새로운 B를 만듬

`cat "A" >> "B"` A의 내용을 B의 내용 끝에 연결

## git 명령어 (커밋)

`git init` 현재 디렉터리에서 깃을 사용할 수 있도록 저장소로 초기화

`git init " "` 디렉터리를 만들고 저장소로 초기화

`git status` 깃 상태 확인

`git add " "` 스테이징

`git add .` 작업트리에서 수정한 모든 파일을 스테이징

`git commit -m "message"` 커밋, 메시지 등록

`git log` 버전 확인
>커밋 해시 commit<br>
>만든 사람 Author:<br>
>만든 시각 Date:<br>
>커밋 메시지 " "<br>

`git log --stat` 커밋과 관련된 파일(통계)까지 보기

`git log --oneline` 한줄에 한 커밋씩 보여줌

`git commit -am "message"` 스테이징과 커밋 동시에 처리

`git diff` 수정 사항 보기

`git restore " "` 작업트리에서 수정한 파일 되돌리기

`git restore --staged " "` 스테이징 되돌리기

`git reset --soft HEAD^` 커밋 취소, 스테이지로 되돌리기

`git reset --mixed HEAD^` `git reset HEAD^` 커밋 취소, 스테이지 취소, 작업 디렉터리에 보관

`git reset --hard 해시값` 해시값(커밋id)를 최신 버전으로 만듬(상위 버전은 전부 삭제)

`git revert 해시값` 해당 커밋을 삭제하고, 취소했다는 커밋을 새로 만듬

## git 명령어 (브랜치)
`git branch` 브랜치 확인

`git branch " "` 브랜치 만들기 (분기)

`git switch " "` 브랜치 전환

`git log --oneline` 간결하게 커밋 보기

`git log --branches` 브랜치마다 최신 커밋 보기

`git log --graph` 브랜치 그래프 형태로 표시

`git log --oneline --branches --graph` `git log --oneline --all --graph` 간결하게 브랜치마다 최신 커밋 그래프로 보기

`git merge " "` 브랜치 병합

`git branch -d " "` 병합된 브랜치 감추기(삭제)

`git branch -D " "` 병합 하지 않은 브랜치 강제 감추기(삭제)

`git cherry-pick 헤시값` 헤시값 버전을 최신 버전으로 올리기(체리픽)

