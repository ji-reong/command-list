## 브랜치 관리

### 현재 위치한 브랜치 확인
```Shell
#예시: git branch
```

### 브랜치 생성
```Shell
git branch {생성하려는 브랜치의 이름}
#예시: git branch test
```

### 브랜치 이동
```Shell
// 구 버전 명령어) git checkout {이동하려는 브랜치의 이름}
// 신 버전 명령어) git switch {이동하려는 브랜치의 이름}
#예시: git switch test
```

## 업로드와 다운로드

### 로컬 저장소의 변경 사항을 원격 저장소에 업로드
```Shell
git push {원격 저장소의 이름 또는 주소} {브랜치의 이름}
#예시: git push origin test
```

### 원격 저장소의 변경 사항을 로컬 저장소에 업데이트
```Shell
git fetch {원격 저장소의 이름 또는 주소} {브랜치의 이름}
#예시: git fetch origin test
```
- fetch는 마지막 pull 이후 원격 저장소에 생긴 변경 사항을 다운로드합니다.
- 원격 저장소에서 변경 사항이 발견된 경우, merge나 rebase를 수행하여 로컬 저장소에 이를 업데이트해야 합니다.

### 원격 저장소의 변경 사항을 로컬 저장소에 업데이트 + 병합
```Shell
git pull {원격 저장소의 이름 또는 주소} {브랜치의 이름}
#예시: git pull origin test
```
- git pull은 원격 저장소에 생긴 변경 사항을 다운로드하고 이를 로컬 저장소에 바로 병합합니다.
- 일반적으로, pull로 인해 로컬 저장소에서 작업 중인 내용이 날아가는 것을 방지하기 위하여 pull을 하기 전에 fetch를 수행합니다. 

## 충돌 관리

### 다른 브랜치로 merge
```Shell
git merge {병합의 target이 되는 브랜치}
#예시: git merge main
```
- test 브랜치를 main으로 병합하고 싶다면 `git switch test`를 입력하여 test 브랜치로 이동한 후, `git merge main`을 입력하면 됩니다.