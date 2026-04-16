<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=2563EB&center=true&vCenter=true&width=700&lines=BOM-Based+Inventory+Management;Automotive+Parts+Cost+%26+Stock+Tracking;Vue+3+%2B+Spring+Boot+%2B+MySQL)](https://git.io/typing-svg)

</div>

# 🚗 BOM 기반 자동차 의장 공정 재고 관리 시스템

## 프로젝트 소개

Auto BOM Inventory는 자동차 의장 공정에서 사용되는 부품, 자재, 주문 정보를 통합적으로 관리하기 위한 웹 기반 재고 관리 시스템입니다.

자동차 의장 공정은 다양한 부품이 조립되는 복잡한 공정이기 때문에, 부품 정보와 재고 상태, 주문 현황을 체계적으로 관리하는 것이 중요합니다. 본 프로젝트는 BOM 데이터를 기반으로 자재 상태와 주문 정보를 연계하여, 재고 부족 여부를 파악하고 데이터 기반 의사결정을 지원하는 것을 목표로 합니다.

## 주요 기능
<img width="1919" height="865" alt="image" src="https://github.com/user-attachments/assets/50f094b8-0b25-4caf-894f-365a9d48e03b" />
   

### 1. 로그인 및 회원가입

- 이메일과 비밀번호 기반 로그인
- 사용자 상태에 따른 로그인 제한
  - `Active`: 로그인 가능
  - `Pending`: 승인 대기
  - `Deleted`: 비활성화 상태
- 회원가입 시 비밀번호 암호화 저장
- 기본 회원가입 계정은 `User` 권한과 `Pending` 상태로 생성

---
   
<img width="1919" height="865" alt="image" src="https://github.com/user-attachments/assets/29de27a4-b06d-49ef-97b7-6c4b1ebe0629" />

### 2. 권한 관리

- 관리자 계정만 접근 가능한 권한 관리 페이지 제공
- 사용자 역할 변경
  - `User`
  - `Admin`
- 사용자 상태 변경
  - `Active`
  - `Pending`
  - `Deleted`
- 이름 및 사번 기준 사용자 검색
- 승인 대기 사용자 관리
---
<img width="1919" height="868" alt="image" src="https://github.com/user-attachments/assets/ceec026d-f4f7-4140-a342-86f46fd10940" />

### 3. BOM 조회

- 자동차 의장 공정 부품 정보 조회
- 부품 카테고리별 테이블 제공
- BOM 및 가격 검색 기능
- 페이지네이션 적용
- API를 통한 BOM 데이터 연동
---
<img width="1919" height="868" alt="image" src="https://github.com/user-attachments/assets/79d3051e-0430-4f71-b50f-03c98a7e2255" />

### 4. 자재 관리

- 최신 재고 현황 조회
- 재고 변동 이력 관리
- 전체 자재 수, 정상 자재 수, 주문 필요 항목 수 확인
- 부족 자재 경고 상태 표시
- 입고 및 출고 처리
- 실제 재고와 시스템 재고 차이 발생 시 재고 조정 가능
---
<img width="1919" height="865" alt="image" src="https://github.com/user-attachments/assets/70376ccf-6400-4949-9b6e-6f3f7b11f18b" />

### 5. 주문 현황

- 전체 주문 건수 및 주문 상태 집계
- 차종별 주문 비율 차트 제공
- 주문 상세 데이터 조회
- 조건별 필터링
- 필터링된 데이터 CSV 다운로드
- 페이지네이션 적용
---
## 기술 스택

### Frontend

![Vue.js](https://img.shields.io/badge/Vue.js-3-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-Markup-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-Style-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Vue Router](https://img.shields.io/badge/Vue_Router-Routing-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)
![Pinia](https://img.shields.io/badge/Pinia-State_Management-FFD859?style=for-the-badge)
![Axios](https://img.shields.io/badge/Axios-API_Client-5A29E4?style=for-the-badge&logo=axios&logoColor=white)

### Backend

![Spring Boot](https://img.shields.io/badge/Spring_Boot-Backend-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Java](https://img.shields.io/badge/Java-Language-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![MyBatis](https://img.shields.io/badge/MyBatis-SQL_Mapper-BF0000?style=for-the-badge)
![REST API](https://img.shields.io/badge/REST_API-Architecture-009688?style=for-the-badge)

### Database/Deployment

![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Aiven](https://img.shields.io/badge/Aiven-Cloud_DB-FF5722?style=for-the-badge)
![Vercel](https://img.shields.io/badge/Vercel-Frontend_Deploy-000000?style=for-the-badge&logo=vercel&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-Collaboration-181717?style=for-the-badge&logo=github&logoColor=white)


## 시스템 구조

```text
Frontend (Vue 3)
        ↓ Axios
Backend (Spring Boot REST API)
        ↓ MyBatis
Database (MySQL / Aiven DB)
```
## DB 설계

본 프로젝트의 데이터베이스는 BOM, 가격, 재고, 주문, 사용자 정보를 중심으로 구성했습니다.

### 주요 테이블

| Table | Description |
| --- | --- |
| `user` | 사용자 계정 및 권한 정보 |
| `bom` | 부품 기본 정보 |
| `price` | 부품별 가격 정보 |
| `storage` | 자재 재고 정보 |
| `orders` | 주문 정보 |

### 주요 관계

- `bom.part_id`를 기준으로 가격, 재고, 주문 정보를 연결
- `price.part_id`는 부품별 가격 정보를 관리
- `storage.part_id`는 부품별 재고 정보를 관리
- `orders.part_id`는 주문 대상 부품 정보를 참조
- `user.employee_id`는 사용자 계정을 식별하는 기본키로 사용

---
## 실행 방법

### 1. Repository Clone

서브모듈을 포함하여 clone합니다.

```bash
git clone --recurse-submodules https://github.com/your-username/auto-bom-inventory.git
cd auto-bom-inventory
```

이미 clone한 경우에는 다음 명령어로 서브모듈을 초기화합니다.

```bash
git submodule update --init --recursive
```

### 2. Frontend 실행

```bash
cd frontend
npm install
npm run dev
```

### 3. Backend 실행

```bash
cd backend
./mvnw spring-boot:run
```

Windows 환경에서는 다음과 같이 실행할 수 있습니다.

```bash
mvn spring-boot:run
```
---

## 협업 규칙

### Branch Strategy

```text
main      : 배포용 브랜치
develop   : 개발 통합 브랜치
feature/* : 기능 단위 개발 브랜치
```

### 작업 흐름

```text
develop 브랜치에서 feature 브랜치 생성
→ 기능 개발
→ commit
→ Pull Request 생성
→ 코드 리뷰
→ develop 브랜치에 merge
→ 테스트 후 main 브랜치에 merge
```

### Commit Convention

커밋 메시지는 다음 타입을 사용합니다.

| Type | Description |
| --- | --- |
| `feat` | 새로운 기능 추가 |
| `fix` | 버그 수정 |
| `docs` | 문서 추가 및 변경 |
| `style` | 코드 포맷팅 |
| `refactor` | 코드 리팩토링 |
| `test` | 테스트 코드 추가 및 수정 |
| `chore` | 빌드, 패키지 매니저 등 기타 작업 |
| `move` | 파일 이동 |
| `rename` | 파일 이름 변경 |
| `remove` | 파일 삭제 |
| `design` | UI 디자인 수정 |

예시:

```bash
feat: add bom page
fix: update login validation
docs: update README
chore: add frontend and backend submodules
```

---

## 팀원 역할

| Name | Role |
| --- | --- |
| 이온유 | 팀장, 프로젝트 기획, 일정 관리, 협업 규칙 및 브랜치 전략 선정, BOM 조회 페이지 구현, BOM 테이블 설계 및 데이터 생성 |
| 김수민 | 커밋 컨벤션 정의, 로그인 및 회원관리 페이지 구현, `user` 테이블 설계 및 데이터 생성 |
| 김민재 | BOM 및 차량별 모듈 카테고리 선정, 주문 현황 페이지 구현, `orders` 테이블 설계 및 데이터 생성 |
| 표성중 | 페이지별 요구사항 분석, 자재 관리 페이지 구현, `price` 및 `storage` 테이블 설계 및 데이터 생성 |

---

## 프로젝트 기간

```text
2026.04.09 ~ 2026.04.17
```

| Period | Task |
| --- | --- |
| 04/09 ~ 04/10 | 주제 선정, 협업 규칙 선정, 팀 역할 분담, 요구사항 분석, 자료조사, API 명세서 작성 |
| 04/10 ~ 04/13 | UI/UX 설계, ERD 설계, DB 테이블 구현 및 데이터 선정 |
| 04/13 ~ 04/14 | Frontend 구현, Backend 구현, DB 배포 |
| 04/15 ~ 04/16 | 코드 리팩토링, 기능 테스트, Frontend 및 Backend 배포 |
| 04/17 | 발표자료 제작 |

---

## Demo

```text
https://vue-pjt-frontend.vercel.app/#/login
```

---

## 기대 효과

- BOM 기반 부품 정보 통합 관리
- 자재 부족 상태의 빠른 파악
- 주문 현황 및 진행 상태 시각화
- 관리자의 사용자 권한 및 상태 관리
- 자동차 의장 공정의 자재 관리 프로세스 디지털화
