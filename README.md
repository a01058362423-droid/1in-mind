# 1in-mind

1인 기업(솔로 창업가)이 사업 운영과 앱 개발을 동시에 해나가기 위한 Claude Code 스킬/커스텀 명령어 모음.

## 구성

### `.claude/skills/` — 사업 운영

| 스킬 | 용도 |
|---|---|
| `one-person-business-plan` | 비즈니스 모델·타겟 고객·수익 구조를 1페이지로 정리 |
| `landing-page-copy` | 랜딩페이지 헤드라인/카피 작성 |
| `pricing-strategy` | 요금제·가격 정책 설계 |
| `pitch-deck` | 투자/세일즈용 피치덱 작성 |
| `launch-content` | 플랫폼별 런칭/홍보 게시물 작성 |
| `customer-support-macros` | 고객 문의 응대 템플릿 |
| `solo-decision-framework` | 공동창업자 없이 혼자 결정 내릴 때의 사고 프레임 |

### `.claude/skills/` — 앱 개발

| 스킬 | 용도 |
|---|---|
| `product-spec` | 아이디어를 경량 PRD(스펙)로 정리 |
| `app-architecture-planner` | 솔로 개발자용 기술 스택·아키텍처 설계 |
| `release-checklist` | 출시/배포 전 점검 체크리스트 |

### `.claude/commands/` — 빠른 실행용 슬래시 명령어

`/launch-post`, `/spec`, `/pricing`, `/pitch`, `/release-check` — 위 스킬들을 즉시 호출하는 단축 명령어.

## 왜 이렇게 구성했는가

각 스킬은 하나의 책임만 가지도록 좁게 스코프를 잡았다(범용 "비즈니스 도우미" 하나가 아니라 용도별로 분리). 이렇게 하면 Claude가 요청 의도에 맞는 스킬만 정확히 불러오고, 각 스킬의 지침이 서로 충돌하지 않는다.
