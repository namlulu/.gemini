# Antigravity Global Rules

## 1. 언어 설정 (Language Preference)
- 사용자와 소통할 때는 항상 **한국어**로 정중하고 명확하게 답변해 주세요. (Always respond and communicate with the user in Korean).
- 다만, 코드 작성이나 에러 메시지 분석 등 기술적인 컨텍스트에서는 필요에 따라 영어를 병행하여 사용할 수 있습니다.

## 2. 코드 품질 및 구현 지침 (Coding & Implementation Guidelines)
- **코드 무결성 유지**: 기존 코드에 작성되어 있는 무관한 주석(Comments)이나 문서화 주석(Docstrings)은 임의로 삭제하거나 수정하지 않고 그대로 유지해 주세요.
- **최소 주의 원칙**: 기능 구현 시 불필요하게 복잡하거나 거대한 코드를 작성하지 말고, 요구사항에 딱 맞는 직관적이고 재사용 가능한 최소한의 코드로 구현해 주세요.
- **임시 파일 사용**: 디버깅이나 일회성 스크립트 실행이 필요할 경우, 프로젝트 루트 폴더를 어지럽히지 말고 `<appDataDir>/brain/<conversation-id>/scratch/` 디렉토리를 활용하여 작업해 주세요.

## 3. 도구(Tools) 및 환경 관리
- **안전한 명령 실행**: 시스템에 위험을 초래할 수 있는 임의의 파괴적 명령(예: `rm -rf /` 등)은 절대 실행하지 않아야 하며, 명령 실행 전에 항상 영향도를 검토해야 합니다.
- **민감 정보 보호**: API 키나 개인 로컬 환경 경로가 포함된 파일(예: `.env`, `mcp_config.json`)을 다룰 때는 절대 소스 관리(Git)에 노출되지 않도록 주의해 주세요.

## 4. Google Antigravity 공식 문서 참고 (Google Antigravity Documentation Reference)
- 개발 및 에이전트 동작 시 다음 공식 문서를 참고하세요:
  - **공식 문서 홈**: [Google Antigravity Docs](https://antigravity.google/docs)
  - **CLI 개요**: [Antigravity CLI Overview](https://antigravity.google/docs/cli-overview)
  - 에이전트가 터미널 환경, 샌드박스, 설정(settings.json) 등을 변경 혹은 이해해야 할 때는 위 문서와 하위 및 관련 문서의 사양을 최우선으로 참고하여 작업을 수행합니다.
