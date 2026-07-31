<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.zh-CN.md">中文</a> ·
  <a href="README.ja.md">日本語</a> ·
  <a href="README.ko.md"><strong>한국어</strong></a>
</p>

<h1 align="center">glue-coding-skill: 다시 만들지 말고, 검증된 능력을 연결하세요</h1>

<p align="center"><strong>Codex용 Skill입니다. 성숙한 SDK / API / 프레임워크 / 플랫폼 기능을 먼저 재사용하고, 얇은 glue code와 품질 게이트로 AI 코딩 결과를 안정화합니다.</strong></p>

<p align="center">
  <a href="LICENSE"><img alt="MIT" src="https://img.shields.io/badge/license-MIT-2ea44f?style=for-the-badge"></a>
  <img alt="Codex Skill" src="https://img.shields.io/badge/Codex-Skill-111827?style=for-the-badge">
  <img alt="AI Coding" src="https://img.shields.io/badge/AI%20Coding-Workflow-2563eb?style=for-the-badge">
</p>

## 왜 필요한가요?

AI는 코드를 매우 빠르게 작성할 수 있습니다. 하지만 인증, 큐, 스케줄러, 로깅, 스토리지, SDK 래퍼 같은 일반 기능까지 실수로 새로 만들기 쉽습니다.

`glue-coding`은 Codex에 다음 원칙을 심어 줍니다.

> 공통 문제는 성숙한 기능으로 해결한다. glue code는 비즈니스 흐름을 연결한다. 커스텀 코어 코드는 기본값이 아니라 예외다.

## 무엇을 도와주나요?

- 공식 SDK, API, 관리형 서비스, 안정적인 오픈소스를 먼저 찾기
- 유지보수 상태, 문서, 라이선스, 보안, 이전 비용 평가하기
- 도메인 로직과 외부 의존성 분리하기
- 짧고 얇고 테스트 가능하며 삭제하기 쉬운 glue code 작성하기
- 테스트, schema, 오류 처리, 관측성, 롤백 경로 확인하기

## 설치

```powershell
git clone https://github.com/KumiKo2007/glue-coding-skill "$env:USERPROFILE\.codex\skills\glue-coding"
```

사용 예:

```text
Use $glue-coding to design this feature with mature capabilities first.
```

## 잘 맞는 작업

- 기능 기획
- 아키텍처 리뷰
- AI 생성 코드 리팩터링
- API / SDK 통합
- 직접 만들지, 구매할지, 감쌀지, 삭제할지 결정하기

## License

MIT.