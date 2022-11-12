# 📌 OMDb API를 활용한 영화 검색 사이트 만들기

## 결과물

- 배포 사이트: [https://sjh-movie-search.netlify.app](https://sjh-movie-search.netlify.app)
- 참고한 사이트
  - [https://stupefied-hodgkin-d9d350.netlify.app/#/](https://stupefied-hodgkin-d9d350.netlify.app/#/)
  - [https://grep.app/](https://grep.app/)
    <br/>

## 기술 스택

<img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/> <img src="https://img.shields.io/badge/scss-CC6699?style=for-the-badge&logo=sass&logoColor=white"> <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white">
<img src="https://img.shields.io/badge/babel-F9DC3E?style=for-the-badge&logo=babel&logoColor=black"> <img src="https://img.shields.io/badge/postcss-DD3A0A?style=for-the-badge&logo=postcss&logoColor=white">
<br/>

## 요구사항

### :exclamation: 필수

- [x] 영화 제목으로 검색 가능하고 검색된 결과의 영화 목록이 출력돼야 합니다.
- [x] jQuery, React, Vue 등 JS 라이브러리와 프레임워크는 사용하지 않아야 합니다.
- [x] 스타일(CSS) 라이브러리나 프레임워크 사용은 자유입니다.
- [x] 실제 서비스로 배포하고 접근 가능한 링크를 추가해야 합니다.

### :grey_question: 선택

- [x] 한 번의 검색으로 영화 목록이 20개 이상 검색되도록 만들어보세요.
- [x] 영화 개봉연도로 검색할 수 있도록 만들어보세요.
- [x] 영화 목록을 검색하는 동안 로딩 애니메이션이 보이도록 만들어보세요.
- [ ] 무한 스크롤 기능을 추가해서 추가 영화 목록을 볼 수 있도록 만들어보세요.
- [x] 영화 포스터가 없을 경우 대체 이미지를 출력하도록 만들어보세요.
- [x] 단일 영화의 상세정보(제목, 개봉연도, 평점, 장르, 감독, 배우, 줄거리, 포스터 등)를 볼 수 있도록 만들어보세요.
- [x] 영화 상세정보가 출력되기 전에 로딩 애니메이션이 보이도록 만들어보세요.
- [ ] 영화 상세정보 포스터를 고해상도로 출력해보세요.(실시간 이미지 리사이징)
- [x] 차별화가 가능하도록 프로젝트를 최대한 예쁘게 만들어보세요.
- [ ] 영화와 관련된 기타 기능도 고려해보세요.<br/>

## 추가 기능

- 무한 스크롤 대신 페이지네이션 구현
- Checkbox를 활용한 영화 목록 변화
- 사용자의 편의를 위해 movie, series, episode 의 개수를 출력
- 영화 찾기에서 오류 발생 시 오류 화면 출력<br/>

## 아쉬운 점 / 어려웠던 점

- SPA를 사용하지 않고 여러 페이지를 만든 점이 아쉽다.
- 쿼리스트링을 사용하고 싶었으나 쿼리가 바뀔 시 주소가 새로고침 되어 화면전체가 다시 출력되는 것을 어떻게 해결하는지 몰라서 사용하지 않은 점이 아쉽다.
- 모듈화를 하지 않은 점이 가장 아쉽다. 한 파일에 작업을 몰아서 하다보니 막상 모듈화를 하려고 할 때 너무 막막해서 포기한 점이 아쉽다.
- 영화 목록을 최신 순 혹은 평점 순으로 정렬을 하고 싶었으나 OMDb API는 최신 순이나 평점 순으로 정렬하는 기능을 제공하지 않아서 아쉬웠다.
- 프로젝트 구조를 너무 더럽게 만든 것 같다
- 전체적으로 코드를 너무 더럽게 짠 것 같다.
- search 페이지에서 검색어가 바뀔 시 영화 목록도 바로 바뀌도록 만들었는데 여기서 검색어로 "cat" 입력 시 "c", "ca", "cat" 이렇게 3개의 검색 결과가 순차적으로 나오는 문제가 있었다. 이를 해결하기 위해 setTimeout과 clearTimeout을 사용했는데 좀 억지 느낌이 났다. 더 나은 해결방법이 있는지 궁금하다.
- 잘 구현되었다고 생각했었는데 예상치 못한 버그가 발견된 경우가 많았다. 이러한 버그를 찾는 것이 중요하다고 느꼈다. 지금도 발견하지 못한 버그들이 있을 수 있는데 찾아주시면 감사하겠습니다.
으로 영화 목록이 20개 이상 검색되도록 만들어보세요.
