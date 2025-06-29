# 🧩 MatchingBot 

## 🧩 MatchingBot은 AI 기반 HR 매칭 플랫폼

![MatchingBot](images/MatchingBot.png)

AI 기반 이력서-채용공고 매칭 서비스를 개발한 팀 프로젝트입니다.  
본 프로젝트에서 **백엔드 주요 기능 개발 및 API 설계**를 담당했습니다.

---

## 📌 주요 기능 (담당 파트)

- **채용공고 검색 필터링 기능 개발**
    - 직군 → 직종 → 직무 선택 구조 구현 (다단계 직무 선택 UI)
    - 지역 필터링 API 설계
    - 동적 JPQL 기반 검색 쿼리 작성 (Spring Data JPA 활용)


![Search](images/Search.png)
![SearchPosting](images/SearchPosting.png)

- **지도 기반 채용공고 표시 기능**
    - Kakao Map API 연동
    - 내 위치 기반 반경 내 채용공고 마커 표시
    - 주소 검색 기반 마커 표시 및 상세 페이지 이동 처리

![Map](images/Map.png)


- **커뮤니티 게시판 CRUD 기능**
    - 게시글 작성/수정/삭제, 댓글 작성 기능
    - 회원 유형에 따른 권한 제어 (로그인 여부에 따른 권한 처리)

![Community](images/Community.png)

- **챗봇 메뉴 이동 기능**
    - Spring Security 기반 사용자 권한별 챗봇 응답 처리
    - GPT API 연동 (기본 질의응답 및 페이지 이동 지원)

![ChatBot](images/ChatBot.png)

---

️- **코드 스니펫 추가**  

java
@GetMapping("/api/jobs/search")
public ResponseEntity<List<SearchPostingDto>> searchJobs(
@RequestParam String jobRoleName,
@RequestParam String region,
@RequestParam String careerType) {
return ResponseEntity.ok(searchPostingService.searchJobs(jobRoleName, region, careerType));
}

## ERD
![ERD](images/ERD.png)

## Git
![Git](images/Git.png)

## 기술스택
![기술 스택](images/Language.png)

---

## 서비스 아키텍처
![서비스 아키텍처](images/Service.png)


## 🧑‍💻 주요 학습 및 경험

- 실전 협업 환경에서의 Git 브랜치 전략, PR 병합 충돌 해결
- API 설계, DB 스키마 설계, ERD 작성 및 테이블 설계
- 외부 API 통합 및 실시간 지도 서비스 구현
- LLM 기반 AI 기능 적용 경험

---

