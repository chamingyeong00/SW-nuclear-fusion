# 🤝 SW-nuclear-fusion 협업 가이드

## 브랜치 전략
- `master`: 최종 제출용
- `develop`: 통합 개발 브랜치
- `feature/{이슈번호}-{기능요약}`: 기능 단위 작업 브랜치

---

## 작업 흐름

### 1️⃣ 이슈 작성
- GitHub Issues에 작업할 이슈 생성  
- 생성된 이슈 번호 확인 (예: #7)

### 2️⃣ 브랜치 생성
**항상 develop 최신을 기준으로 작업 시작**  
`feature/{이슈번호}-{기능요약}` 브랜치 생성  

```bash
git checkout develop       # develop 브랜치로 이동
git pull                   # 최신 develop 코드 받아오기
git checkout -b feature/7-home-ui  # 새 feature 브랜치 생성 및 이동
```

### 3️⃣ 기능 구현 및 커밋  
`[커밋타입/#이슈번호] - 커밋내용`  
`[feat/#7] - 홈 화면 UI 레이아웃 추가`

### 4️⃣ 원격 브랜치 Push
'git push origin feature/7-home-ui'

### 5️⃣ 코드 확인 후 Merge  
	• GitHub로 이동 → Pull Request 생성
	• PR 작성 시:
		• base: develop
		• compare: feature/7-home-ui
	• PR 생성 후 팀원이 코드 리뷰 진행
	• 리뷰 완료 후 Merge 버튼 클릭하여 develop 브랜치에 병합

### 6️⃣ 최종 제출 시 `develop` → `master` merge
  git checkout master
  git pull
  git merge develop
  git push origin master

## 커밋 컨벤션

형식: `[커밋타입/#이슈번호] - 커밋내용`

| 타입 | 설명 |
|---|---|
| feat | 기능 추가 |
| fix | 버그 수정 |
| docs | 문서 수정 |
| refactor | 리팩토링 |
| style | 스타일 수정 |
| test | 테스트 작성 |
| chore | 설정 수정 |
| build | 빌드 수정 |
| ci | CI/CD 설정 |

## 이슈 라벨 가이드

| 라벨 | 설명 |
|---|---|
| Feature | 새로운 기능 |
| BugFix | 버그 수정 |
| Html&css | 마크업/스타일 |
| CrossBrowsing | 브라우저 호환성 |
| Accessibility | 접근성 |
| API | API 문제 |
| Docs | 문서 작업 |
| Deploy | 배포 문제 |
| Setting | 개발 환경 |
| Refactor | 리팩토링 |
| Test | 테스트 관련 |
