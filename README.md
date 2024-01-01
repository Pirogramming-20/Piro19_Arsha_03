# 과제 3 - Arsha 클론코딩 (3조)

## 조원

김연우, 이주형, 이진혁, 정예진

## 협업

### 역할분담

[제목 없는 데이터베이스](<%E1%84%80%E1%85%AA%E1%84%8C%E1%85%A6%203%20-%20Arsha%20%E1%84%8F%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A9%E1%86%AB%E1%84%8F%E1%85%A9%E1%84%83%E1%85%B5%E1%86%BC%20(%E1%84%90%E1%85%B5%E1%86%B7%20%E1%84%80%E1%85%AA%E1%84%8C%E1%85%A6)%20ffc608d4adb740d796175e54fe62ba2f/%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%82%E1%85%B3%E1%86%AB%20%E1%84%83%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%90%E1%85%A5%E1%84%87%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%89%E1%85%B3%20d608a71cefc7425e9ef1b53599d89692.csv>)

- 협업 규칙
  - main 브랜치 보호 규정
    - pr 이후 approve를 받아야 main에 merge할 수 있도록 설정
  - 브랜치 이름 통일
    - (기능 이름)/(브랜치 생성자 이름)
    - ex. animation/jinhyeok
  - 전체 모임 시간에 merge

## 구현 상세

### 헤더

- 최상위 헤더
  - 고정영역 구현: position fixed로 구현
  - 호버 애니메이션
- 헤더
  - multiple drop down header 구현
  - 스크롤 내리면 색이 나타나는 애니메이션: animation-timeline: scroll();로 구현
  - 고정영역 구현: position fixed로 구현
  - 호버 애니메이션
  - drop box, deep drop box 애니메이션
- 메인
  - 이미지 아래위로 운동하는 애니메이션: infinite alternate-reverse both 로 구현
- 배너
  - 호버, 스케일 애니메이션 구현

### 메인

- ABout us
  - 버튼 호버 애니메이션 구현
- 아코디언 (eum, faq)
  - input type radio 통해서 한 번에 하나의 박스만 열리도록 구현
  - 질문에 hover 했을 때 색이 바뀌도록 답안이 열렸을 때와 닫혔을 때 따로 구현
  - answer가 열릴 때 부드럽게 열리도록 애니메이션 구현
- 프로그레스 바
  - postion absolute 사용하여 배경바, 진행바 겹침.
  - 진행바 확장 애니메이션 구현
  - 스크롤 이동 시 옆쪽에서 들어오는 애니메이션 구현
- Team
  - 카드 컴포넌트 생성
  - Hover 애니메이션 구현
- Call to action
  - 배경 사진이 스크롤에 따라 이동하도록 고정 (background fixed)
  - 버튼 hover 애니메이션 구현
  - 스크롤 이동 시 전체 div zoom in 애니메이션 구현
- portfolio
  - input type radio 라디오 버튼을 사용하여 하나만 선택할 수 있는 select button bar 구현
  - checked 상태에 따라 사진 필터링
  - 사진 레이아웃 트랜지션 애니메이션 구현
    - display none → inline-block 상태에서의 애니메이션은 구현하지 못함.
  - 스크롤 이동 시 컴포넌트가 fade up 되는 애니메이션 구현
- pricing
  - 카드 컴포넌트 grid로 구현, nth-chile(2)로 2번째 상자 다르게 하기
  - 같은 view point여도 entry 수치를 달리하여 순차적으로 올라오는 애니메이션 구현
  - 기타 호버 및 디테일 추가
- contact
  - iframe태그로 지도 삽입
  - textarea태그로 가변형 input form 삽입
  - 기타 호버 및 디테일 추가
- newsletter 및 footer
  - position : absolute로 서치버튼 왼쪽 정렬
  - 기타 호버, 크기 등 디테일 추가

### 기타

- 스크롤 애니메이션
  - animation-timeline:view()이용해서 구현
  - 스크롤을 내렸을 때 종류별로 적절한 애니메이션 보이도록 함.
    - fade up, expandImg, moveFrom Side
- 최상단 이동 버튼 (gototop)
  - top 버튼을 만들고 눌렀을 때 메인 화면 위치로 이동하도록 구현
  - hover 기능도 함께 구현
  - 가장 위 페이지에서는 안 보이다가 조금 내렸을 때부터 보이기 시작하도록 애니메이션 구현
