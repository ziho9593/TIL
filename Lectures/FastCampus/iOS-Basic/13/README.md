## Chapter 13. TODO List 앱
<p align="center"><img src=./result.gif width="24%"> </p>

- Any.do 스타일 앱 - Task Page / Settings Page
- iOS에서 데이터 저장 방법: NSCoding, Property List, Serialization, Core Data, Realm 등
- Codable
    - NSCoding 처럼 간단하고 적은 데이터를 관리하기에 매우 적합한 기능들을 제공
    - 'JSON'을 쉽게 다룰수 있게 도와줌
    - NSCoidng 보다 덜 복잡하며 훨씬 직관적이면서도, 더 손쉽게 사용 가능
- 정리하면, 데이터를 결국 파일의 형태로 디스크를 이용해 관리하는 것
- 'Tab Bar Controller'를 사용해 화면 하단에 위치한 각 Tab Bar의 Controller 구성 가능
- TableView를 'Static Cells'를 활용해 직접 커스텀 가능
- 객체 간의 동등비교를 하기 위해선 'Equatable'이라는 프로토콜을 따라야 함
- JSON 타입은 현업에서 가장 많이 쓰이는 데이터 타입
    - let json: [String: Any] 형태로 Swift에서 사용
    - Swift에서는 'Codable' 덕분에 JSON 파일을 Struct 형태로 아주 쉽게 파싱이 가능
    - Codable 프로토콜은 'Decodable'과 'Encodable'이 합쳐진 형태