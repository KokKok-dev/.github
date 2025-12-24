# 🍽️ TableKok : MSA 기반 음식점 통합 예약 플랫폼

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/925e2a68-f38e-45da-b033-8aa31a764219" />


> **"고객과 점주 모두를 위한 올인원 예약 솔루션"** > 일반 예약부터 인기 맛집 실시간 대기열(Queue), 현장 웨이팅까지 한 번에 관리하는 MSA 기반 서비스입니다.

<br>

## 📖 프로젝트 소개
**TableKok**은 음식점 예약, 웨이팅, 리뷰 관리를 하나의 플랫폼에서 제공하여 파편화된 예약 경험을 통합합니다.
단순한 예약 기능을 넘어, **대규모 트래픽이 발생하는 인기 맛집의 대기열 처리**와 **실시간 현장 웨이팅** 문제를 기술적으로 해결하는 데 초점을 맞추었습니다.

### 🧑‍💻 팀원 구성

| 이름 | 역할 | 담당 도메인 및 기여 | GitHub |
|:---:|:---:|:---|:---:|
| **태성원** | 팀장 | 🔐 Auth, 🚪 Gateway(Auth), 🏗 Infra | [Link](https://github.com/trevivom76) |
| **이가현** | 부팀장 | 🏪 Store, ⏳ Waiting | [Link](https://github.com/gashine20) |
| **송준일** | 팀원 | 🔍 Search, ⭐ Review, 🚪 Gateway(Routing) | [Link](https://github.com/thdwnsdlf61) |
| **황교석** | 팀원 | 📅 Reservation(Normal/Queue) | [Link](https://github.com/gyoseok17) |


### 📅 프로젝트 기간
* 2025.11.24 ~ 2025.12.26(5주)


### 🌟 핵심 목표
* **사용자 경험 통합:** 예약, 웨이팅, 리뷰를 하나의 앱에서 처리
* **대용량 트래픽 처리:** 인기 맛집 예약 시 발생하는 동시성 이슈 및 서버 부하 해결
* **실시간성 보장:** SSE와 Kafka를 활용한 실시간 알림 및 데이터 동기화
* **검색 성능 최적화:** Elasticsearch + Nori 분석기를 이용한 빠르고 정확한 한글 검색

<br>

## 🧬 인프라 설계도

### [인프라 아키텍처]
<img width="1801" height="1131" alt="image" src="https://github.com/user-attachments/assets/b0e66817-fdc2-4d1b-ad6c-169a24ee4d5c" />

### [CI/CD]
<img width="11007" height="1172" alt="image" src="https://github.com/user-attachments/assets/c2e1e2b9-03a9-4336-ac1b-629e72201708" />

### [시스템 아키텍처]
<img width="2148" height="1481" alt="image" src="https://github.com/user-attachments/assets/a1748c4b-1f0e-40f9-baa7-921beb485790" />

### [ERD]
<img width="1791" height="1186" alt="image" src="https://github.com/user-attachments/assets/d1676138-aa69-4004-858b-13975852b2a3" />

<br>

## 🛠 기술 스택 (Tech Stack)
![Java](https://img.shields.io/badge/Java-17-007396?style=flat-square&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.5.8-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-ORM-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Spring Cloud](https://img.shields.io/badge/Spring_Cloud-MSA-6DB33F?style=flat-square&logo=spring&logoColor=white)

![Kafka](https://img.shields.io/badge/Apache_Kafka-Event_Driven-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-Caching_&_Queue-DC382D?style=flat-square&logo=redis&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-Search_Engine-005571?style=flat-square&logo=elasticsearch&logoColor=white)
![SSE](https://img.shields.io/badge/SSE-Realtime-000000?style=flat-square&logo=html5&logoColor=white)

![AWS EC2](https://img.shields.io/badge/Amazon_EC2-Compute-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![AWS RDS](https://img.shields.io/badge/Amazon_RDS-Database-527FFF?style=flat-square&logo=amazon-rds&logoColor=white)
![AWS ECS](https://img.shields.io/badge/Amazon_ECS-Container-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![AWS ECR](https://img.shields.io/badge/Amazon_ECR-Registry-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Container-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI%2FCD-2088FF?style=flat-square&logo=github-actions&logoColor=white)

![JMeter](https://img.shields.io/badge/Apache_JMeter-Performance_Test-D22128?style=flat-square&logo=apachejmeter&logoColor=white)
![JitPack](https://img.shields.io/badge/JitPack-Library_Dist-81C784?style=flat-square&logo=jitpack&logoColor=white)

![Slack](https://img.shields.io/badge/Slack-Communication-4A154B?style=flat-square&logo=slack&logoColor=white)
![Discord](https://img.shields.io/badge/Discord-Communication-5865F2?style=flat-square&logo=discord&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-Team_Space-000000?style=flat-square&logo=notion&logoColor=white)

| 구분 | 기술 (Technology) |
|:---:|:---|
| **Language & Framework** | Java 17, Spring Boot 3.2, Spring Cloud (Gateway, Eureka, OpenFeign) |
| **Database** | PostgreSQL, Redis (Caching, Pub/Sub, ZSet), Elasticsearch |
| **Message Queue** | Apache Kafka (Event-Driven Architecture) |
| **DevOps & Infra** | Docker, Zipkin (Distributed Tracing), GitHub Actions (CI/CD) |
| **Tools** | QueryDSL, SSE (Server-Sent Events), JWT |

<br>

## 서비스별 포트번호
| 서비스명 | 포트번호 |
|:---:|:---:|
| **Eureka Server** | 19090 |
| **API Gateway** | 19091 |
| **User-service** | 8081 |
| **Store-service** | 8082 |
| **Search-service** | 8083 |
| **Reservation-service** | 8084 |
| **Hot-Reservation-service** | 8085 |
| **Waiting-service** | 8086 |
| **Review-service** | 8087 |

<br>
