# 💬 Talk & Deal - 사용자 참여형 커뮤니티 플랫폼

> Final Project | 2025.10 - 2025.11 | 팀 4명

자유게시판 · 투표 · 중고거래 기능을 갖춘 사용자 참여형 커뮤니티 플랫폼입니다.

## 🛠 기술 스택
- **Backend**: Java 17, Spring Boot 3.5, Spring Security, JWT, MyBatis
- **Frontend**: React 18, Recoil, React-Router, Axios Interceptor, React-Quill
- **Database**: Oracle 11g XE
- **Tools**: VS Code, Eclipse, GitHub Desktop

## 👤 담당 기능 (이용재)
- **자유게시판 CRUD**: 카테고리/서브카테고리 동적 필터링 (MyBatis `<if>` 태그 단일 쿼리)
- **댓글 시스템**: 본문과 댓글 API 분리로 비동기 로딩, 응답 속도 개선
- **좋아요 (Optimistic UI)**: 클릭 즉시 UI 반영 후 서버 동기화, 실패 시 롤백. 토글 방식 단일 API
- **추천글 사이드바**: 동일 카테고리·서브카테고리 내 좋아요 수 기준 상위 10개 추출 (ROWNUM)
- **XSS 방어**: DOMPurify로 React-Quill 에디터 출력 시 악성 스크립트 제거

## 📐 아키텍처
React Client (CSR/Recoil) → Axios/JWT → Spring Boot (Security → Controller → Service → DAO) → MyBatis → Oracle

## 🔗 Links
- [포트폴리오](https://leeyongjae-portfolio.vercel.app)
