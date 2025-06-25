# 🤝 SW-nuclear-fusion 협업 가이드

## 브랜치 전략

- `master`: 최종 제출용
- `develop`: 통합 개발 브랜치
- `feature/{이슈번호}-{기능요약}`: 기능 단위 작업 브랜치

## 작업 흐름

1️⃣ 구현할 기능 Issue 작성  
2️⃣ `feature/{이슈번호}-{기능요약}` 브랜치 생성  
3️⃣ 기능 구현 및 커밋  
4️⃣ Pull Request → `base: develop`  
5️⃣ 코드 확인 후 Merge  
6️⃣ 최종 제출 시 `develop` → `master` merge

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
