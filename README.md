> [!NOTE]
> 🎯 Date: 2026년 9월 12일  
> 이 프로필은 3개월 후 내가 이루고 싶은 모습과 목표를 바탕으로 작성되었습니다.  
> 현재의 상황과는 다를 수 있지만, 앞으로 나아갈 방향과 지향점을 담고 있습니다.

<br/><br/>

# 👋 AI 기술을 서비스로 실현하는 Applied AI / Backend 엔지니어 이혜원입니다.

> 💡 **5년 차 백엔드 엔지니어**로서 탄탄한 백엔드 인프라(Kubernetes) 기술력을 바탕으로,
> **복잡한 AI 에이전트 워크플로우 설계(LangGraph), 구조화 데이터 추출 최적화, 그리고 소형 LLM 파인튜닝 파이프라인 수립**을 주도하며 프로덕션 레벨의 AI 시스템을 구축하고 있습니다.

<br><br>

## 🚀 About Me
- 💼 **경력**: 2021. 10 ~ 현재 (재직중)
- 🎯 Backend Engineer → AI System Engineer 로 역량 확장 중
- 🤖 Gemini 기반 AI 서비스 상용화 프로젝트 수행
- 🏛️ AI 국가 과제 기술 제안 및 인프라 아키텍처 설계 참여
- ☸️ Kubernetes 기반 서비스 운영 및 배포 환경 구축 경험

<br/><br/>

## 💻 주요 프로젝트 경험

### 소형 LLM 기반의 자율적 지식 추출 및 자가 교정(Self-Correction) 멀티 에이전트 시스템 구축 (2026.06 ~ 2026.09)
- **개요:** 자원 제한적 환경(CPU 서버)에서 소형 모델을 활용해 비정형 기술 문서로부터 고정밀 구조화 데이터(Pydantic/JSON 지식 그래프)를 안정적으로 추출하는 Fault-Tolerant 파이프라인 설계
- **주요 수행 역할 및 엔지니어링 성과:**
  - **LangGraph 기반 장기 실행 워크플로우 설계:** 모델의 출력 오류(JSON 깨짐, 필수 필드 누락) 발생 시 시스템 다운타운 없이 에러 컨텍스트를 유지하며 최대 3회 자동 재시도하는 자가 교정(Self-Correction) 조건부 루프 구현.
  - **Structured Output & 예외 복구(Human-in-the-loop):** 연속 리트라이 실패 시 Persistent Checkpointer(PostgreSQL 기반)를 활용해 태스크 상태를 고정하고, 엔지니어 개입(Interrupt/Resume)을 통해 데이터를 수동 교정 후 중단점부터 재개하는 장애 복구 메커니즘 수립.
  - **로컬 데이터 수집 기반 소형 LLM 파인튜닝 (MLOps):** 자가 교정 루프에서 누적된 '실패 프롬프트-성공 JSON' 데이터셋 500건을 가공하여 Google Colab(QLoRA/Unsloth)에서 `Qwen2.5-3B` 모델을 파인튜닝. **JSON 포맷팅 성공률을 68%에서 94%로 개선하며 파이프라인의 전체 Latency를 40% 단축.**
  - **LLM Observability 환경 구축:** 리눅스 네이티브 환경에 **LangSmith**를 연동하여 에이전트의 노드별 실행 속도, 토큰 소모량, 툴 호출 실패율을 실시간으로 추적 및 모니터링할 수 있는 가시성 체계 설계.

### 국책 과제(국가 사업) 아키텍처 설계 및 인프라 빌드업 (2026 ~ 현재)
- **AI 관련 국가 과제 기술 제안서 작성 및 기획 참여** (과제 최종 선정).
- **고성능 AI 인프라 아키텍처 설계 및 검토**
  - 인공지능 모델 서빙 인프라 고도화를 위해 **DGX 및 Spark 클러스터 이중화, 네트워크 스위치 및 미디어 서버 배치**를 포함한 고가용성(HA) 인프라 아키텍처 초안 설계.
  - 실무 담당자로서 벤더사 기술 조율(하드웨어 견적 및 스펙 세부 검토) 수행 중.

### AI 서비스 상용화 및 대기업 프로젝트 (2025)
- **실시간 대시보드 데이터를 LLM 컨텍스트로 변환**
  - 대시보드 내 실시간 데이터를 분석 및 컨텍스트화하여 사용자 요구사항에 맞게 답변하는 **Gemini API 기반 대화형 채팅 시스템** 개발 담당.
  - 실제 비즈니스 데이터와 LLM을 연동하는 백엔드 파이프라인 설계 및 대화형 인터페이스 최적화 수행.

### 2021 ~ 2024 주요 프로젝트
- 신세계 면세점 배리어프리 키오스크 개발
- LG 원격 로그 업로드 시스템 'LAUS' 개발
- LG 모바일 관제 Kubernetes 환경 구축
- LG 앱 업그레이드 시스템 'AUS' 개발
- LG 배송로봇 주문 결제 서비스 '클로이 오더' 개발 및 유지보수

<br/><br/>

## 🛠 기술 스택 및 역량

### 🚀 핵심 실무 역량

실제 서비스 개발 및 운영 경험을 기반으로 가장 자신 있게 활용하는 핵심 기술입니다.
#### Backend 엔지니어링
<a href="#-backend--core" style="pointer-events: none; cursor: default;">![JAVA](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADIAAAAyCAYAAAAeP4ixAAAACXBIWXMAAAsTAAALEwEAmpwYAAAE0UlEQVR4nN2ae4hVVRTGt5bWpGVTY2ZRjTpQaKUihNUfTRZmTu8HDT2oICR72R9jRllUUySR+odl9A6rKdSCXlZUFFSGvewNPaeEXkipRFKW84vFfIfW3Z57vXfuubdz++DAmbvPOXt/e++11rfWnhDqDGBc+D8AuATYIzQ6gJuBC0OjA3gPuD80MoDT6MeK0KgAxgHrRWRRaEQAY4Cv+BcnhEYDMAn4wZH4EtghNBKAE4FNjkQfMLPE87sBI0JeAAwCrge2Uohbo+cOAC4HngJ6gWuBISEPAJqA5WwLG+xgPTMdeNm1fQRMDHkBsBewJoXE68BwYCSwKmq7E9gp5AXACGBtCok3gF2BQyKj/wu4LOQJwI7Aqykk3pEB27XO/b4ZmBHyBuDSFBKf21ZS+41RW2fII4C3o4FusCDo2i12JFgb8grg54jIxa5tZ8WPBC+GvIJCT7XFBu/ahgB/u/bfzGZCHgFc4Qb6a0q7uV+P7pBHAM3R9poctbdHRH4HRoc8AjjdDfTRlPbHIjK3hbwCWOyCXWvU1gL86Ih8EfIKYLCthga6JKV9liOyPuQZ9JNZrOgdr8p+jsiq0AgArgSeiH471Lnoqf/l4IYDxwNzgaWS6yuVU0yOMz9LooAp7u8HtFJnlehjAnCHYpO57SWmqrMiYFviceAPtzU2Ahf54Ffk3SQHORW4D2gr8twuJudtpYALoiD7dSaZI/Ah26JXgdBWaIquA4GxKjaM1P1EDW6mykHnaAVvAR5SgvWuxZpQ2Kcpgmdcf3OzILKM2uElYJ8i/U51z63IKgc/CXhE8tyLwHJhseV7JVr3Al3AcfbtEv0emymRlA4sURoPnALMU3zwVydwsgZiTmB0YisV9rPAEbmhFkQsSj8sN3pMDfP/DW4127LuYKjJCzdT36iMcyQwqsjqjdHqzJLnsvc/BY4qEVSfc31cnSkJV+5ZV4Y9JLNZCn2yl6GRPS513+nKnEQ0y/OBTxgYfgJ6LDD6JIv+ONKjwt7zpgRqRiKF1N5ABzAHWAjcLcm+XALSonS3Yse0pCCR8p1hwDXyZmPrRkCdm0d6QfJ8u6VOO3IDzpMiqNiL1QSSLZuisudCicXEDXdJCa9UJcXHH4sn4+s54BbgCMWMTt2bQR5O9Xg/zdMlKBUsK902z8pz+Fx7jfZ8s4z1gwoH/5m80vTtDRR4sCp7AY6W3PYwQ2wq8vyeVgIFZsubLdDVLcl/tlawpYIx7C6F/Uo1RMzTePTV05MAba56+Vo1H5om+eFhs3Nd5lKh0P3OkOv+0xXzqsskFRt81cPjW8WJm6w8aoebsqlRxdyw8gsTjwebNFFuYh7uHmC1G3yCp4GDUlRF+0DINCmQrU45RisXmyM3XQq9Vu+KC3zuUNUcS0fFRKIP2WyfYeeAVojWcXM8i+Vii4SjecXb5db3L9LvJMkWqx/3VEWiBDlTqfsqnW1XrDlTlwXE83XfofYJkueDyohd50o19Gk3LMrsWFsDb9Wx82y56eYMvtsqsvMV8ZPq/VYdoh6WCYESCthW4C7Z0MfKv5cphsxz1xyt0FWyActJntR7G1O23Zt6r6DAVxeImHkj+38s01w2k2/JFn6x4wapBLMru/9OEsUqJTYZdnxn22/YQAbwD0ShtPhilnUGAAAAAElFTkSuQmCC)</a>&nbsp;
<a href="#-backend--core" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"></a>&nbsp;
<a href="#-backend--core" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white"></a>&nbsp;
<a href="#-backend--core" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"></a>&nbsp;
<a href="#-backend--core" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"></a>&nbsp;
<a href="#-backend--core" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"></a>

#### 데이터베이스
<a href="#%EF%B8%8F-database--modeling" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"></a>&nbsp;
<a href="#%EF%B8%8F-database--modeling" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"></a>&nbsp;
<a href="#%EF%B8%8F-database--modeling" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white"></a>&nbsp;
<a href="#%EF%B8%8F-database--modeling" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black"></a>&nbsp;
<a href="#%EF%B8%8F-database--modeling" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/ERwin%20(Data%20Modeling)-4479A1?style=for-the-badge&logo=databricks&logoColor=white"></a>

#### DevOps 및 인프라
<a href="#%EF%B8%8F-devops--infrastructure" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white"></a>&nbsp;
<a href="#%EF%B8%8F-devops--infrastructure" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/VMware-607078?style=for-the-badge&logo=vmware&logoColor=white"></a>&nbsp;
<a href="#%EF%B8%8F-devops--infrastructure" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"></a>&nbsp;
<a href="#%EF%B8%8F-devops--infrastructure" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white"></a>&nbsp;
<a href="#%EF%B8%8F-devops--infrastructure" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Apache%20Tomcat-F8DC75?style=for-the-badge&logo=apachetomcat&logoColor=black"></a>&nbsp;
<a href="#%EF%B8%8F-devops--infrastructure" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white"></a>

> **주요 역량**
>
> - Java · Spring Boot 기반 백엔드 서비스 설계 및 개발
> - Node.js 기반 API 서버 및 비즈니스 로직 구현
> - Kubernetes 및 Jenkins 기반 배포·운영 환경 구축
> - RDBMS 설계 및 ERD 모델링

<br/>

### 🤖 AI 엔지니어링 및 MLOps

AI 서비스 상용화와 AI 시스템 엔지니어링 역량 확장을 위해 집중하고 있는 기술 분야입니다.

#### AI 엔지니어링 및 MLOps (실무 수준 활용)
![LangChain](https://img.shields.io/badge/LangChain-7FC8FF?style=for-the-badge&logo=langchain&logoColor=black)
![LangGraph](https://img.shields.io/badge/LangGraph-7FC8FF?style=for-the-badge&logo=langgraph&logoColor=black)
![Ollama](https://img.shields.io/badge/ollama-FFA500?style=for-the-badge&logo=ollama&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white)
![LangSmith](https://img.shields.io/badge/LangSmith-01233F?style=for-the-badge&logo=langchain&logoColor=white)
![Hugging_Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)

> **AI 엔지니어링 핵심 역량**
>
> - **LangGraph State Management:** 복잡한 에이전트의 비동기 처리, 조건부 라우팅, 메모리 지속성(Persistence) 설계
> - **Structured output & Tool calling:** Pydantic 스키마를 통한 LLM 출력 형식 강제 및 외부 시스템 연동 안정화
> - **Observability & Evaluation:** LangSmith 기반 LLM Trace 분석 및 에이전트 품질 정량 평가
> - **LoRA/QLoRA Fine-tuning:** Hugging Face 및 PEFT 라이브러리를 활용한 다운스트림 태스크용 소형 모델 최적화

<br/>

### ⚡ 활용 기술

프로젝트 수행과 협업 과정에서 활용한 기술들입니다.

#### Frontend
<a href="#-frontend--tools" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black"></a>&nbsp;
<a href="#-frontend--tools" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white"></a>&nbsp;

#### 협업 및 생산성 도구
<a href="#-version-control--collaboration" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"></a>&nbsp;
<a href="#-version-control--collaboration" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"></a>&nbsp;
<a href="#-version-control--collaboration" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/GitLab-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white"></a>&nbsp;
<a href="#-version-control--collaboration" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Bitbucket-0052CC?style=for-the-badge&logo=bitbucket&logoColor=white"></a>&nbsp;
<a href="#-version-control--collaboration" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white"></a>&nbsp;
<a href="#-version-control--collaboration" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Confluence-0052CC?style=for-the-badge&logo=confluence&logoColor=white"></a>

#### 개발 환경 및 운영체제
<a href="#%EF%B8%8F-environment--os" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/Rocky%20Linux%209.5-11B48A?style=for-the-badge&logo=rockylinux&logoColor=white"></a>&nbsp;
<a href="#%EF%B8%8F-environment--os" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/CentOS%208-262577?style=for-the-badge&logo=centos&logoColor=white"></a>&nbsp;
<a href="#%EF%B8%8F-environment--os" style="pointer-events: none; cursor: default;">
![Windows](https://img.shields.io/badge/Windows%2010%2F11-0078D4?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAeCAYAAAA7MK6iAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAmklEQVR4nO3WoQ0CQRBA0U2oAIekBySODhBYHBUg0Cg6IMFj6ICEAjCYsxSAIUFhUA+FIwd3LNlcbr/feZtRE0KuqaGLASZYYIMDLrGAMeZYY48zHkoKMX5dBlSGUeD+zePY8McyXKWQ4fbC7UuqVcvwmzLceLhIcgi8Qg9DTLHEFkdc/wonO/bqhg76GGGGFXY44VZ7cC780BOinanoCy2MrwAAAABJRU5ErkJggg==)
</a>

> **추가 경험**
>
> - 프론트엔드와 백엔드를 아우르는 Full-Stack 개발 경험
> - Linux 서버 운영 및 트러블슈팅
> - Git 기반 협업 및 프로젝트 관리

<br/><br/>

## 📜 자격증 및 지속적인 학습

<a href="#-certifications--continuous-learning" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/정보처리기사-2023.09 취득-326CE5?style=for-the-badge&logo=qiskit&logoColor=white"></a>&nbsp;
<a href="#-certifications--continuous-learning" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/SQLD%20(SQL%20개발자)-2026.09%20취득-326CE5?style=for-the-badge&logo=databricks&logoColor=white"></a>&nbsp;
<a href="#-certifications--continuous-learning" style="pointer-events: none; cursor: default;"><img src="https://img.shields.io/badge/CKA%20(Kubernetes)-🔜%20준비%20중-EAB308?style=for-the-badge&logo=kubernetes&logoColor=white"></a>

> **💡 자격증 취득 계획**
> * ~~🗓️ **SQLD (SQL 개발자):** 2026년 8월 22일 시험 응시 예정 (9월 11일 합격 발표)~~
> * 🗓️ **CKA (Certified Kubernetes Administrator):** 2026년 12월 9일 이내 응시 완료 예정

<br/><br/>

## 🎓 학력

- **서울여자대학교 (Seoul Women's University)**
  - **주전공**: [디지털미디어전공](http://dm.swu.ac.kr/%eb%94%94%ec%a7%80%ed%84%b8%eb%af%b8%eb%94%94%ec%96%b4%ed%95%99%ea%b3%bc/%ed%95%99%ea%b3%bc%ec%86%8c%ea%b0%9c/) (Major in Digital Media, B.S. in Engineering)
  - **복수전공**: [정보보호전공](http://security.swu.ac.kr/sub.html?page=introduce_division) (Major in Information Security, B.S. in Engineering)
  - **부전공**: [소프트웨어융합전공](http://sw.swu.ac.kr/%ec%86%8c%ed%94%84%ed%8a%b8%ec%9b%a8%ec%96%b4%ec%9c%b5%ed%95%a9%ed%95%99%ea%b3%bc/%ED%95%99%EA%B3%BC%EC%86%8C%EA%B0%9C/) (Minor in Software Fusion)
