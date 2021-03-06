## Chapter 05. Swift Function and Optional

### Function
- 어떠한 기능을 수행하는 코드 블록
- Method와 기능을 수행한다는 점에서 비슷
- Method는 Object에 속하는 반면, Function은 독립적
- object.methodName() vs. funtionName()
- 파라미터 이름 앞에 _ 혹은 external name을 붙여 사용 가능
- 파라미터에 default 값을 설정할 수 있음
- 반환하는 값의 타입도 func 줄 끝에 '-> type'으로 명시해줘야 함

### Function 고급기능
- Overload는 같은 함수 이름이지만, 파라미터나 리턴이 달라지는 경우 사용
- 파라미터는 넣는 순간 복사되어 함수 안에서 상수로 사용되므로 직접 변경 불가
- 변경하기 위해선 외부의 변수를 사용하기 위한 inout을 붙여야 함 (type 앞에)
- inout 파라미터에 값을 넣어 함수를 사용할 땐, 값 앞에 &를 붙여야 함
- 함수 자체를 변수에 할당하여 사용할 수 있음
- 함수는 값뿐만 아니라 함수 자체를 파라미터로 넘길 수도 있음
- 함수를 파라미터로 넘길 때 중요한 것은 같은 타입의 함수를 넘겨야 한다는 것
- 함수는 될 수 있으면 한 가지 기능만 가능하도록 구성하는 것이 좋음 (순수함수)
- 최대한 순수함수로 남겨두기 위해서 가능하면 10줄 내외로 작성하는 것이 좋음
- 함수 코드가 길어지면 그 안에서 또 다른 함수들로 나눠주는 것이 좋음

### Optional
- Swift는 Optional이라는 기능으로 값이 있거나 없을 수도 있음을 동시에 표현 가능
- Optional은 type 뒤에 ?을 붙여 선언함으로 사용
- 값이 '없다'라는 것은 'nil'이라는 단어로 표현

### Optional 고급기능
- Forced unwrapping : 억지로 박스를 까보기
- -> 옵셔널 변수를 호출할 때 뒤에 !를 붙여 사용, nil을 호출하면 에러 발생
- Optional binding (if let) : 부드럽게 박스를 까보자 1
- -> if let 으로 값이 있는 경우엔 할당, 없는 경우는 else로 처리
- Optional binding (guard) : 부드럽게 박스를 까보자 2
- -> guard let 으로 조건 검사를 진행하여 맞지 않는 경우 else문 실행 및 종료
- Nil coalescing : 박스를 까봤더니, 값이 없으면 디폴트 값을 줘보자
- -> 옵셔널이 아닌 타입을 지정 후, 뒤에 ?? 와 디폴트 값을 작성