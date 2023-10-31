# 매우쉽게 알려주는 git & github
## 목차
- [git add, commit으로 파일 기록해놓을 수 있음](#git-add-commit으로-파일-기록해놓을-수-있음)
- [git add, commit, diff 쉽게 하는 법](#git-add-commit-diff-쉽게-하는-법)
## git add, commit으로 파일 기록해놓을 수 있음
- `git init`
    - 작업 폴더에서 git을 쓰기 위해 사용
- `git add 파일명`
    - 기록을 남길 파일을 선택함
- `git commit -m '메세지`
    - 파일의 변경사항을 기록함
- Staging
    - `init`한 폴더에서 기록을 남길 파일을 `add`하는 것을 `staging`이라고 함
    - `staging`한 파일 중에서 `commit`된 파일들은 `repository(저장소)`로 옮김
- `git add .`
    - 모든 파일을 `add`함
- `git status`
    - 어떤 파일들을 staging 했는지, 어떤 파일들이 수정됐는지 알려줌
- `git log --all --oneline`
    - commit 내역 조회
## git add, commit, diff 쉽게 하는 법
- 요즘엔 터미널로 명령어를 직접 치기보단 에디터(ex. vscode)에서 제공하는 기능을 사용하여 쉽게 add, commit을 할 수 있음
- `git diff`
    - 최근 commit과 현재 파일에 차이점을 보여줌
- `git difftool`
    - Vim 에디터를 이용하여 좀 더 비주얼적으로 보여줌
- `git difftool 커밋아이디`
    - 현재 파일과 커밋 아이디에 해당하틑 파일을 비교해줌
    - 커밋 아이디 : `git log --all --oneline`를 했을 때 커밋 메세지 옆에 있는 기호조합
- git difftool도 불편함, 에디터의 확장 기능을 활용하여 더 쉽고 간편하게 git diff를 사용할 수 있음
## git의 branch 만들기
