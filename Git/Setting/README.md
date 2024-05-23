## 설정 정보 조회

### 글로벌 설정 (전역 설정)
```
git config --list --global
```

- 여러 저장소에서 두루두루 쓰이는 정보

### 지역 설정 (지역 설정)
```
git config --list --local
```

- 해당 저장소에만 쓰이는 정보

### 해당 리포지토리의 원격 저장소 주소 조회
```
git remote -v
```
- v 옵션: verbose. 자세하게 출력.
