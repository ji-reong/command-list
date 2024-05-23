## 브랜치 관리

### 현재 위치한 브랜치 확인
```
git branch
```

### 브랜치 생성
```
git branch {생성하려는 브랜치의 이름}
#git branch test
```

### 브랜치 이동
- 구 버전 명령어
```Shell
git checkout {이동하려는 브랜치의 이름}
# git checkout test
```

- 신 버전 명령어
```Shell
git switch {이동하려는 브랜치의 이름}
# git switch test
```

### 브랜치 삭제
- 작업 내역이 없을 때
```Shell
git branch -D {삭제하려는 브랜치의 이름}
# git branch -D test
```
- 삭제하려는 브랜치 이외의 브랜치에서 위 명령어를 입력해야 합니다.