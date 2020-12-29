##-breakpoints란 

​	**브레이크포인트**(breakpoint), **중단점**, **중지점**은 개발에서 프로그램을 의도적으로 잠시 또는 아예 멈추게 하는 장소를 가리키며 디버깅 목적으로 넣는 것이다. 코드 변수의 상태를 확인하거나 특정 중단점에서 호출 스택을 확인할 수 있습니다. 



##watch사용법 

Expresstion 에 parameter 이름을 적고나서 브레이크 포이트를 찍어 놓거나  Step over / Step into/ Step out 을 하면서 변수에 저장된 정보를 확인한다.



##call stack 의 의미 

자바스크립트는 단일 스레드 프로그래밍 언어이므로, 단일 호출 스택이 있습니다. 단일 호출 스택이 있다는 뜻은 한 번에 하나의 일(Task)만 처리할 수 있다는 뜻입니다.



호출 스택이란 프로그램에서 우리가 어디에 있는지를 기본적으로 기록하는 데이터 구조입니다. 동작 방식은 다음과 같습니다. 함수를 실행하면 해당 함수의 기록을 스택 맨 위에 추가(Push) 합니다. 우리가 함수를 결과 값을 반환하면 스택에 쌓여있던 함수는 제거(Pop) 됩니다. 

```javascript
function multiply(x, y) {
    return x * y;
}
function printSquare(x) {
    var s = multiply(x, x);
    console.log(s);
}
printSquare(5);
```



![9995544C5C32151627](C:\Users\DELL\Desktop\9995544C5C32151627.png)





참고 문헌 :  [https://new93helloworld.tistory.com/358]





##Step over / Step into/ Step out 

- step over : 한줄을 실행합니다. 함수가 있어도 실행 후 다음으로 넘어갑니다.
- step into : 함수 내부로 들어갑니다.
- step out : 함수를 끝까지 실행시키고 호출시킨 곳으로 되돌아 갑니다.