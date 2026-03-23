# NewsBrief README (Markdown)

# NewsBrief: AI-Powered Daily News Digest

## 프로젝트 소개

NewsBrief는 주요 언론사의 헤드라인을 수집하여 LLM(대형 언어 모델)을 통해 3줄 요약을 제공하는 자동화 페이지 생성 도구입니다. 바쁜 현대인들과 개발자들을 위해 맞춤형 뉴스 레터를 생성합니다. 테스트 수정

## 주요 기능

- 실시간 크롤링: 국내외 주요 뉴스 사이트의 RSS 및 HTML 파싱
- AI 요약: GPT-4 또는 오픈소스 LLM을 활용한 핵심 요약
- 카테고리 분류: 정치, 경제, IT, 스포츠 등 자동 분류
- 다양한 출력: 웹 페이지(HTML), 마크다운, PDF 지원

## 기술 스택

| 분야 | 기술 | 비고 |
| --- | --- | --- |
| Language | Python 3.10+ | 고성능 비동기 처리 |
| Framework | FastAPI | Others | 뉴스 API 서버 구축 |
| Database | PostgreSQL | 뉴스 데이터 적재 |
| Deployment | Docker / GitHub Actions | CI/CD 파이프라인 |
| Summarizer | OpenAI API / LangChain | AI 텍스트 요약 |

## 설치 및 실행 방법

### 1. 저장소 가져오기 (Clone)

앞서 배운 대로, 기여를 원하신다면 먼저 Fork 후 아래 명령어를 입력하세요.

```bash
# 본인의 계정에서 clone 하세요
git clone https://github.com/YourID/NewsBrief.git
cd NewsBrief
```

### 2. 의존성 설치

본 프로젝트는 Poetry를 사용하여 패키지를 관리합니다.

```bash
poetry install
poetry shell
```

매일 쏟아지는 뉴스 홍수 속에서 핵심만 골라 읽으세요. AI가 취합하고 요약하는 가장 스마트한 방법.

### 3. 환경 변수 설정

`.env.example` 파일을 복사하여 `.env` 파일을 생성하고 API 키를 입력하세요.

## 기여 방법 (Contribution)

이 프로젝트는 BlueMoon님과 같은 기여자들의 참여를 환영합니다!

- Issue를 먼저 생성하고 작업 의사를 밝혀주세요.
- 브랜치명은 `feat/이슈번호-기능명` 형식을 권장합니다.
- PR 본문에는 작업 내용과 테스트 결과를 포함해 주세요.

## 정책 및 행동 강령

본 프로젝트는 커뮤니티의 건강한 문화를 위해 다음 정책을 준수합니다.

- Code of Conduct: 서로 존중하고 예의를 지켜주세요.
- Security Policy: 보안 취약점 발견 시 비공개로 보고해 주세요.
- Contributing Guide: 상세한 기여 절차를 확인하세요.

## 연락처 및 저작권

- Author: BlueMoon (@YourGitHubID)
- License: 본 프로젝트는 MIT License를 따릅니다.

## 오늘의 개발 팁

GitHub Actions를 활용하면 매일 아침 8시에 뉴스를 자동으로 요약하여 이메일로 보낼 수 있습니다. `workflows/daily_digest.yml` 파일을 참고해 보세요!

주의: 절대 API 키가 포함된 `.env` 파일을 GitHub에 Push하지 마세요!

“코드 한 줄의 수정이 누군가의 아침을 바꿉니다.” — NewsBrief Maintainer