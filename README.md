# SSH KEY 인증

1. ssh key 생성 (생성 파일의 경로는 ~/.ssh/id_rsa)
- `ssh-keygen -t rsa -C "[GibHub 계정 이메일 주소]"`

3. GitHub Settings 메뉴 이동
- New SSH Key 버튼 클릭
- SSH Key 입력 : `~/.ssh/id_rsa.pub`

4. 생성 완료 후 Generate 확인
- `ssh -T git@github.com`

<br>

# Git 최초 설정


1. Git 전역으로 사용자 이름과 이메일 주소를 설정

~~~git config --global user.name [본인이름]~~~
git config --global user.email [본인이메일]

2. 확인 
- `git config --global user.name`
- `git config --global user.email`

3. 기본 브렌치명 변경
- `git config -global init.defaultBranch main`

4. 기본 편집기 변경하기
- `git config --global core.editor "notepad++"`
- `git config --global core.editor "code --wait"`

5. 에디터에서 config 파일 수정하기
- `git config -e`
- `git config --global -e`

6. 맥에서 숨은 파일 확인 (주로 .gitignore 파일 찾을때 사용..)
- `shift + command + .`

Git 전역으로 사용자 이름과 이메일 주소를 설정
git config --global user.name "본인이름"
git config --global user.email "본인 이메일"

# 확인
git config --global user.name
git config --global user.email

# 기본 브랜치명 변경
git config -global init.defaultBranch main

# 기본 편집기 변경하기
git config --global core.editor "notepad++"
git config --global core.editor "code --wait"

# 맥에서 숨은 파일 확인 (주로 .gitignore 파일 찾을때 사용..)
shift + command + .

# 에디터에서 config 파일 수정하기
git config -e
git config --global -e

