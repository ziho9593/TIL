## 04. 날씨별 옷차림 추천 앱

### 앱 디자인
- 현재 날씨 상황을 나타낼 수 있음
- 위치 별 날씨 상황을 나타낼 수 있음
- 날씨 예상을 조회할 수 있음
- 날씨별 추천하는 옷을 보여줄 수 있음
- 온도별 옷을 다르게 설정할 수 있음

### 데이터 설계
- 날씨 데이터 저장
    - 날짜, 강수 확률, 강수량, 하늘 상태, 습도, 기온, 풍속

### 동네 날씨 예보 OPEN API
- 강수확률, 습도, 강수량, 강수형태, 기온, 풍속 데이터 사용
- 동네 예보 base_time
    - 0200, 0500, 0800, 1100, 01400, 1700, 2000, 2300
    - Base time 이후 10분 뒤 호출 가능
- 하늘 상태
    - 0~5: 맑음
    - 6~8: 구름많음
    - 9~10: 흐림

### 화면 설계
- 메인 화면: 날씨, 옷차림 표현
- 옷차림 변경 화면: 온도에 맞게 옷차림 변경 기능 추가
- 위치 변경하기