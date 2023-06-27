# TravelUS 🚌🧳🚗
🔗[TravelUs 바로가기](https://developer-sala.github.io/icontest/)
- ID: jun123@naver.com
- PW: 123123

### 목차
1. [서비스 소개](#1.-TravelUs-서비스-소개-🚌)
2. [개발 기간](#2.-개발-기간)
3. [팀원 소개](#3.-팀원 소개)
4. [역할 분담](#4.-역할 분담)
5. [프로젝트 목표](#5. 프로젝트 목표)
6. [컨벤션](#6. 컨벤션)
7. [개발 환경](#7. 개발 환경)
8. [폴더 구조]()
9. [주요 기능 및 특징]()
10. [프로젝트 관련 문서]()
11. [프로젝트 소감]()

## 1. TravelUs 서비스 소개 🚌
서비스명 TravelUs는 "Travel"과 "Us"의 합성어로, 함께 여행하자는 의미를 담고 있습니다.
또한 읽을 때, "Travelers"로도 들릴 수 있어 여행자들을 의미하기도 합니다.

저희 서비스는 동행을 원하는 여행자들뿐만 아니라, 여행상품 판매자들, 그리고 새로운 사람들과 만남과 교류를 통해 직간접 여행 경험을 공유하고 싶은 분들에게도 적합한 서비스입니다.
이 서비스를 통해 여행자들을 함께 여행의 즐거움을 공유하고, 여러 사람들과 연결될 수도 있습니다.
- 여행자들은 게시글 작성을 통해 여행에 대한 경험이나, 원하는 여행 상품 동행을 구할 수 있고, 댓글 기능을 통해 서로 소통하며 여행의 즐거움을 공유할 수 있습니다.
- 여행상품 판매자들은 자신의 상품을 등록하고 홍보할 수 있습니다.

## 2. 개발 기간 

## 3. Fearless 4 팀원 소개 <img width="20" src = "https://github.com/starcradle101/starcradle101/assets/113353436/b707fb16-15ec-4e1a-8666-42f08a05be79"> 

Hello, there! 저희는 4명의 Front-End 개발자로 구성된 **Fearless 4** 입니다. 
저희는 모든 팀원이 MBTI F성격 유형이며, 팀원들과 함께라면 어떤 어려움에도 두려움 없이 도전에 임하겠다는 마음으로 팀명을 **Fearless 4**로 정하였습니다.

(<img width="20" src = "https://github.com/FRONTENDSCHOOL5/final-4-/assets/113353436/ed76f0e4-a75a-4db6-9c0d-914a28d20f6d"> LIKELION FE5 Project Team 4)<br>
|**강동훈**|**김소연**|**정준영**|**최사라** |
| :------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| <img width="180" alt="강동훈_profile_img" src="https://github.com/starcradle101/starcradle101/assets/113353436/707efb89-2344-4f79-8080-d3947767a7c5"> | <img width="180"  alt="김소연_profile_img" src="https://github.com/starcradle101/starcradle101/assets/113353436/f3f0197d-2969-4ecf-b907-42b8bc31ade9"> | <img width="180" alt="정준영_profile_img" src="https://github.com/starcradle101/starcradle101/assets/113353436/8661f098-ebe3-4586-a0ab-229bba5532c1"> | <img width="180" alt="최사라_profile_img" src="https://github.com/starcradle101/starcradle101/assets/113353436/db3243c5-1d3b-4010-8547-dabd0034d7eb" > |
| [starcradle101](https://github.com/starcradle101) | [sy412](https://github.com/sy412) | [DayTeaJun](https://github.com/DayTeaJun) | [developer-sala](https://github.com/developer-sala) |
| 팀장 | 팀원 | 팀원 | 팀원 |

## 4. 역할분담 
강동훈
- 게시글 페이지
  
김소연
- 검색페이지
  
정준영
- 프로필 페이지
  
최사라
- 상품페이지
  
공통 작업
- 공통 컴포넌트

## 5. 프로젝트 목표
1. 리액트 사용법을 익히고 실력 향상시키기
   
2. 협업에 필요한 소프트 스킬 기르기
   
3. 누군가와 같이 일하는 프로젝트 환경에 익숙해지기

## 6. 컨벤션 & 브랜치 전략
### 컨벤션
#### 코드컨벤션 
- Prerttierrc : 일관된 코드 스타일 사용으로 개발자들이 코드 스타일을 일일이 조정하거나 협업 중에 스타일 차이로 인한 충돌을 최소화하여 시간절약, 가독성 향상, 유지보수의 용이성 등 개발 프로세스를 더 효율적으로 하기 위해 사용하였습니다.  

.prettierrc 설정
```
{
	"printWidth": 80,
	"tabWidth": 2,
	"useTabs": true,
	"semi": true,
	"singleQuote": true,
	"jsxSingleQuote": true,
	"trailingComma": "es5",
	"bracketSpacing": true,
	"bracketSameLine": false,
	"arrowParens": "always"
}
```

#### 커밋 컨벤션 
```
feat        : 기능 (새로운 기능)  
fix         : 버그 (버그 수정)  
refactor    : 리팩토링  
design      : CSS 등 사용자 UI 디자인 변경  
comment     : 필요한 주석 추가 및 변경  
style       : 스타일 (코드 형식, 세미콜론 추가: 비즈니스 로직에 변경 없음)  
docs        : 문서 수정 (문서 추가, 수정, 삭제, README)  
test        : 테스트 (테스트 코드 추가, 수정, 삭제: 비즈니스 로직에 변경 없음)  
chore       : 기타 변경사항 (빌드 스크립트 수정, assets, 패키지 매니저 등)  
init        : 초기 생성  
rename      : 파일 혹은 폴더명을 수정하거나 옮기는 작업만 한 경우  
remove      : 파일을 삭제하는 작업만 수행한 경우
```

### 브랜치 전략
- GitHubFlow: 비교적 단순하고 직관적인 구조를 가지고 있어, 작은 규모의 단기간 프로젝트에 팀원들이 쉽게 학습하고 적용할 수 있어 이 전략을 선택하였습니다. 


## 7. 기술 스택 
1. 프론트엔드 기술
- <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
- <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white">
- <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
- <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=React&logoColor=black">

2. 백엔드
멋쟁이사자처럼 프론트엔드 스쿨에서 제공된 API 사용

3. 도구 및 라이브러리

<img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white">
<img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">


4. 협업 및 프로젝트 관리

5. 디자인

7. IDE 
|사용 기술|  값2|
|-------|-------|
| 사용 기술   | <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"> <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=React&logoColor=black"> |
| 패키지   | 값4   |
| 포맷터   | 값6   |
| 협업   | 값8   |
| IDE  | 값10  |

이미지 출처
- Splash 화면
"https://kr.freepik.com/free-photo/view-of-adorable-3d-cat_45138557.htm#page=2&query=3d%20cat&position=4&from_view=search&track=ais"
"https://kr.freepik.com/free-psd/travel-luggage-icon-isolated-3d-render-illustration_34151495.htm#query=3d%20BAGGAGE&position=13&from_view=search&track=ais"

- 로그인 화면
"https://kr.freepik.com/free-photo/view-of-adorable-3d-cat_45138557.htm#page=2&query=3d%20cat&position=4&from_view=search&track=ais"
"https://kr.freepik.com/free-photo/love-button-notification-alert-on-chat-speech-bubble-notice-reminder-3d-cartoon-illustration_27654463.htm#query=3d%20heart&position=24&from_view=search&track=ais"

- 채팅 화면 
"https://kr.freepik.com/free-psd/3d-illustration-of-person-with-long-hair_27470372.htm#query=3d%20profile&position=4&from_view=search&track=ais"
"https://kr.freepik.com/free-photo/cute-woman-hold-hands-gesture-to-empty-spec-business-woman-concept-on-pink-background-3d-rendering_25694156.htm#query=3d%20kid&position=25&from_view=search&track=ais"

- 404화면
"https://kr.freepik.com/free-photo/view-of-adorable-3d-cat_45138556.htm#query=3d%20cat&position=43&from_view=search&track=ais"
"https://kr.freepik.com/free-photo/reminder-popup-bell-notification-alert-or-alarm-icon-sign-or-symbol-for-application-website-ui-on-purple-background-3d-rendering-illustration_24598564.htm#query=3d%20alert&position=5&from_view=search&track=ais"

- 기본 프로필 설정 화면 
"https://kr.freepik.com/free-vector/3d-cartoon-young-woman-smiling-in-circle-frame-character-illustration-vector-design_24325541.htm#query=3d%20kid&position=10&from_view=search&track=ais"

- 팔로우한 적이 없는 경우
"https://kr.freepik.com/free-photo/view-of-adorable-3d-cat_45138550.htm#query=3d%20cat&position=8&from_view=search&track=ais"

- 팔로잉한 유저가 없는 경우 
"https://kr.freepik.com/free-photo/view-of-adorable-3d-cats_45138596.htm#page=2&query=3d%20cat&position=10&from_view=search&track=ais"




