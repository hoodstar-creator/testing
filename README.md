# 1학년 2반 디지털컨텐츠과 전용 학습 장소 현황판 (Learning Place Status Board)

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=for-the-badge">
</p>

<p align="center">
  <b>학생들의 실시간 위치 관리와 학급 필수 정보를 한눈에 제공하는 스마트 대시보드</b><br>
  나이스 API 연동 및 다양한 학급 편의 기능을 탑재하고 있습니다.
</p>

---

## 미리보기 (Preview)

<p align="center">
  <img src="https://github.com/hoodstar-creator/testing/blob/main/preview_img.png?raw=true" width="800px" alt="Main Dashboard Screenshot">
</p>
https://dicon-board.vercel.app/
---

## 주요 기능 (Key Features)

<details open>
<summary><b> 실시간 위치 관리 (Magnet Board)</b></summary>
<br>
<ul>
  <li><b>자석 드래그 앤 드롭</b>: 학생 번호 자석을 이동시켜 실시간 위치(등교, 귀교 등) 표시</li>
  <li><b>기타 사유 입력</b>: 독립된 팝업창을 통해 프로젝트실 이용 등 상세 사유 입력 기능</li>
  <li><b>최근 사유 저장</b>: 자주 입력하는 이동 사유를 로컬 저장소에 기억하여 빠른 입력 지원</li>
</ul>
</details>

<details open>
<summary><b> 스마트 학급 정보 (Smart Info)</b></summary>
<br>
<ul>
  <li><b>실시간 날씨</b>: Open-Meteo API를 통해 안산 지역 기온 및 기상 상태 표시</li>
  <li><b>나이스 급식 연동</b>: 교육행정정보시스템(NEIS) API로 오늘의 점심 메뉴 자동 로드</li>
  <li><b>주간 시간표</b>: 학년/반 설정 및 조회 기능 (마지막 설정값 자동 저장)</li>
</ul>
</details>

<details open>
<summary><b> 멀티미디어 & 감성 (Media & Mood)</b></summary>
<br>
<ul>
  <li><b>BGM 플레이어</b>: 감성적인 LP판 디자인의 미니 플레이어 및 리스트 모달</li>
  <li><b>전체 무한 재생</b>: 플레이리스트 전체 곡을 순차적으로 무한 반복 재생</li>
  <li><b>재생 제한 시스템</b>: 수업/자습 시간 자동 차단 로직 및 관리자 암호 우회 기능</li>
  <li><b>배경화면 커스텀</b>: 갤러리 사진을 대시보드 배경으로 설정 (새로고침 시 유지)</li>
</ul>
</details>

---

## 기술 스택 (Tech Stack)

<p align="left">
  <img src="https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black">
</p>

- **Design**: Glassmorphism (Backdrop-filter UI)
- **Data**: NEIS Open API, Open-Meteo API
- **Animation**: HTML5 Canvas (Snow Effect)
- **Storage**: Browser LocalStorage
- **공공API목록**: NEIS 공공데이터 (급식, 시간표), Open-Meteo (날씨)<br>
https://open.neis.go.kr/portal/mainPage.do<br>
https://open-meteo.com/
---

## 설치 및 사용법 (Getting Started)

1. 저장소를 클론합니다.
   ```bash
   git clone [https://github.com/your-username/class-dashboard.git](https://github.com/your-username/class-dashboard.git)
   
2. 별도의 빌드 과정 없이 index.html을 브라우저로 실행하면 즉시 사용 가능합니다.

<details open> <summary><b>⚙️ 설정 가이드 (Configuration)</b></summary>


<code>index.html</code> 상단의 변수를 수정하여 커스텀할 수 있습니다. <ul> <li><code>MEAL_KEY</code>: 나이스 급식 API 키</li> <li><code>TIME_KEY</code>: 나이스 시간표 API 키</li> <li><code>ADMIN_PW</code>: 음악 재생 제한 해제 비밀번호 (기본: 1224)</li> </ul> </details> <br>
## ⚖️ License

Copyright (c) 2025 hoodstar-creator<br>
(Based on the work of Dimigo Class 4)

본 프로젝트는 4반의 소스 코드를 활용하여 제작되었으며, 추가된 모든 기능과 수정 사항은 **MIT 라이선스**를 따릅니다. <br>자세한 내용은 [공식 라이선스 전문](https://opensource.org/licenses/MIT)을 확인하세요.
