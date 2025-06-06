<div  align="center">
  <img src="https://github.com/user-attachments/assets/8d2e9666-6e10-45df-88fa-46c8c295e63e" alt="starmix">
</div>
</br>

- **팀 명 :**  Starmix
- **프로젝트 명 :** checkmate
- **프로젝트 기간 :** 2025.03.06 ~

<div align="center">

| [checkmate](https://checkmate.it.kr) | [checkmate for PM](https://manager.checkmate.it.kr) |
| :---: | :---: |

</div>

</br>

## 🛫 프로젝트 개요
> **소규모 주니어 개발 팀을 위한 프로젝트 관리 및 협업 툴**

AI를 활용한 프로젝트 생성과 Sprint 구성, 회의록 자동 요약 기능을 제공하여 팀의 초기 기획부터 실행까지의 과정을 효율적으로 지원합니다.<br>
회의 내용을 실시간으로 정리할 수 있는 공동 편집 기능을 통해 주요 논의 사항을 요약하고, 이를 실행 가능한 액션 아이템(Task)으로 전환할 수 있습니다.<br>
Task는 Epic 단위로 구조화할 수 있으며, Gantt Chart, Kanban Board, Calendar를 통해 관리할 수 있습니다.<br>
또한 상세 Task 페이지의 댓글 기능을 통해 팀 내부 이해관계자 간의 원활한 소통이 가능하도록 하여, 개발 과정 전반에서 협업의 생산성을 높입니다.

</br>

## 👨‍👩‍👧‍👦 Team

<div align="center">

| 조성연<br>(팀장) | 김평주 | 박승연 | 한도연 |
| :---: | :---: | :---: | :---: |
| <img alt="조성연" src="https://github.com/user-attachments/assets/a7a83797-ae11-4c86-9f9c-f1ee4dcffa37" height="100" width="100"> | <img alt="김평주" src="https://github.com/user-attachments/assets/b8da45f5-20c3-4996-a2f5-79df73a22929" height="100" width="100"> | <img alt="박승연" src="https://github.com/user-attachments/assets/6161e664-bf97-452f-b6b0-6b384a643b7c" height="100" width="100"> | <img alt="한도연" src="https://github.com/user-attachments/assets/106931b7-9abc-4401-bb3e-96cc00dcf838" height="100" width="100"> |
| [@yeonnnnjs](https://github.com/yeonnnnjs) | [@pjookim](https://github.com/pjookim) | [@AstronaCat](https://github.com/AstronaCat) | [@wsd9489](https://github.com/wsd9489) |
| Backend <br> Infra| Frontend <br> FE Lead | AI | Frontend |

</div>

## 🚀 기능 시연
| Solution 1. AI 기반 Sprint Backlog 자동 생성으로 초기 계획 수립 |
| :---: |
| ![sol1](https://github.com/user-attachments/assets/c0d85375-7321-4e42-94fe-e1a0c5c48d0a) |

| Solution 2. 시각화된 프로젝트 진행률 및 작업 상태 공유 |
| :---: |
| ![sol2](https://github.com/user-attachments/assets/07f58706-ca44-4589-8fa7-636d0c5710c9) |

| Solution 3. AI 기반 회의록 요약 및 액션 아이템 도출 후 적용 |
| :---: |
| ![sol3](https://github.com/user-attachments/assets/787590d6-8947-47a2-9fc0-2c541d3898f2) |

| Solution 4. AI 기반 Sprint 자동 재구성으로 Task 우선순위 조정 |
| :---: |
| ![sol4](https://github.com/user-attachments/assets/dccba468-7885-43f4-8b8d-95c39e19c869) |

| Solution 5. Burndown Chart 및 프로젝트 진행 현황 공유 |
| :---: |
| ![sol5](https://github.com/user-attachments/assets/a1421cd4-c4bd-4991-b168-825c44e55b19) |

## Architecture
### Service
<img src="https://github.com/user-attachments/assets/9005a269-6556-43d7-975b-6780ec01e92b">
</br>

### Application
<img src="https://github.com/user-attachments/assets/7829bc5c-8b38-41ea-8c36-7ba2f3b1357c">
</br>

### Infra
<img src="https://github.com/user-attachments/assets/5f855973-c1bc-4fee-a33c-b1ea3f49058b">


### Front-end
[Repository](https://github.com/Starmix-ajou/checkmate-frontend)
| TypeScript | Next.js | Tailwind CSS |
| :---: | :---: | :---: |
| <img alt="TypeScript" src ="https://github.com/user-attachments/assets/5288f3db-96a3-41af-b47e-caeac03277ab" width="65" height="65" /> | <img alt="TypeScript" src ="https://github.com/user-attachments/assets/fa16ac58-00a2-46e1-9295-1552edb6986c" width="65" height="65" /> | <img alt="TypeScript" src ="https://github.com/user-attachments/assets/06f473b2-1f16-4165-92c0-3a94ff2ea161" width="65" height="65" /> | 

#### 특징
| 항목 | 설명 |
|------|------|
| **모노레포 기반 앱 분리** | `apps/web`과 `apps/manager`로 사용자와 관리자 뷰를 분리하여 역할별 개발이 명확하고 독립적인 배포가 가능함. |
| **패키지 단위의 코드 재사용** | `packages/ui`, `packages/types`, `packages/api` 등 공통 모듈을 분리하여 중복 제거와 일관된 인터페이스 유지. |
| **Turborepo로 빠른 빌드와 캐싱 최적화** | 의존성 그래프 기반 병렬 빌드와 캐시를 통해 CI/CD 시간과 로컬 개발 빌드 시간을 크게 단축. |
| **Storybook을 통한 UI 문서화 및 테스트** | 공통 컴포넌트를 시각화하고, 디자인 시스템을 공유하며, UI 테스트를 용이하게 함. |
| **공통 타입과 API 클라이언트로 일관된 통신** | `packages/types`와 `packages/api`를 통해 프론트 전체에서 타입 안정성과 요청 방식 통일성 확보. |
| **역할 중심 브랜치 전략과 협업 흐름** | Jira 이슈 키 기반 브랜치 명명과 디렉토리 기반 작업 분할로 충돌 없는 협업 가능. |
| **배포 파이프라인 시간 단축** | Turborepo와 Vercel을 통한 캐시 및 병렬 빌드로 배포 속도 최적화. |
| **Jest로 유닛 테스트 구현** | 공통 로직과 유틸 함수에 대해 Jest 기반 테스트를 작성하여 기능 안정성과 회귀 방지 보장. |


### Back-end
[Repository](https://github.com/Starmix-ajou/checkmate-backend)
| Java | MongoDB | Spring<br>Boot |
| :---: | :---: | :---: |
| <div style="display: flex; align-items: flex-start;"><img src="https://github.com/user-attachments/assets/0af70e4e-1991-4da1-9eb8-94ee8ab51b73" alt="icon" width="65" height="65" /></div> | <div style="display: flex; align-items: flex-start;"><img src="https://github.com/user-attachments/assets/4821fb33-7da7-497b-9cfc-0ffc0ba436e2" alt="icon" width="65" height="65" /></div> | <img src="https://t1.daumcdn.net/cfile/tistory/27034D4F58E660F616" width="65" height="65" > |

### AI
[Repository](https://github.com/Starmix-ajou/checkmate-ai)
| Python | MongoDB | FastAPI | Hugging Face | OpenAI<br>Chat Completions<br>API |
| :---: | :---: | :---: | :---: | :---: |
| <div style="display: flex; align-items: flex-start;"><img src="https://github.com/user-attachments/assets/1582e55f-96a1-42c9-a038-0677ca66c994" width="65" height="65" /></div> | <div style="display: flex; align-items: flex-start;"><img src="https://github.com/user-attachments/assets/4821fb33-7da7-497b-9cfc-0ffc0ba436e2" alt="icon" width="65" height="65" /></div> | <img src="https://github.com/user-attachments/assets/6e308186-a0f5-4b13-981b-f5029a189505" width="65" height="65" > | <img src="https://github.com/user-attachments/assets/5ec77529-b735-42b5-ac90-827e31b02de3" width="65" height="65" > | <img src="https://github.com/user-attachments/assets/de344faf-a6b4-44eb-bf83-f5f03ff29d13" width="65" height="65" > |

### Infra
| Oracle Cloud | Vercel | Kubernetes | ArgoCD | Atlas MongoDB |
| :---: | :---: | :---: | :---: | :---: |
| <img src="https://github.com/user-attachments/assets/2ad2e3ce-e00e-4893-9f55-8b93b05c14d0" width="85" height="85" /> | <img src="https://github.com/user-attachments/assets/62d996e3-67bf-4ed4-aa4f-d8b44df5ac18" width="65" height="65" /> | <img src="https://github.com/user-attachments/assets/4bd5a357-9174-429d-b88f-d0ccb46332fd" height="50" width="50" > | <img src="https://github.com/user-attachments/assets/a7e614bd-1243-473e-8d18-f3da8e060c0e" width="65" height="65" > | <img src="https://github.com/user-attachments/assets/4821fb33-7da7-497b-9cfc-0ffc0ba436e2" width="65" height="65" > |

### Tools
| Slack | Github | Jira | Notion |
| :---: | :---: | :---: | :---: |
| <img src="https://github.com/user-attachments/assets/47c60780-f844-41f2-b7e5-34096ed97820" width="65" height="65" > | <img src="https://github.com/user-attachments/assets/0f7cd7e5-577c-412c-9362-a0136f71fa5e" width="65" height="65"> | <img src="https://github.com/user-attachments/assets/568ed4a3-c204-4e88-b385-0e422f3e05ef" width="65" height="65"> | <img src="https://github.com/user-attachments/assets/499456f2-c06c-4ccf-99a5-f1c40a7b61e3" width="65" height="65"> |
