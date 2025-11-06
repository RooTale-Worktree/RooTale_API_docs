# LiveTale API Documentation

LiveTale 프로젝트용 API 명세서입니다.

## 📖 API 문서

- **Swagger UI**: [(https://rootale-worktree.github.io/RooTale_API_docs/)]
- **OpenAPI Spec**: [openapi.yml](./openapi.yml)

## 🚀 배포 방법

1. 이 저장소를 GitHub에 푸시
2. GitHub Pages 설정에서 `main` 브랜치 선택
3. 자동으로 배포됩니다

## 📁 파일 구조

```
├── index.html          # GitHub Pages 메인 페이지 (Swagger UI)
├── openapi.yml         # OpenAPI 3.0 명세서
└── README.md           # 프로젝트 설명
```

## 🔧 로컬에서 실행

```bash
# Python HTTP 서버 실행
python3 -m http.server 8000

# 브라우저에서 접속
open http://localhost:8000
```

## 📝 API 엔드포인트 

### POST /story/continue
스토리 이어쓰기 API

**요청:**
```json
{
  "user_input": "string",
  "story_id": "string"
}
```

**응답:**
```json
{
  "reaction_json": {},
  "next_scene": {}
}
```
