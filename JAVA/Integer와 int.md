### 1) int는 무엇인가? (primitive type)

답부터 말한다면, 다음과 같이 말할 수 있습니다.

> int는 변수의 타입(data type)이다.
> 

위의 답을 하나씩 풀어보자면,**변수(variable)는 '값을 저장할 수 있는 메모리 상의 공간'**을 의미 합니다.

int a = 3;char firstName = "H";

에서 a 나 H 는 변수(변수명)가 되는 것입니다.

그리고 그 앞에 적힌 int 와 char가 변수의 형을 지정해주고 있는 것이,변수의 타입( = data type = 자료형 ) 이라 합니다.

즉, **자료형은 'data의 type에 따라 값이 저장될 공간의 크기와 저장 형식을 정의한 것'** 이라고 볼 수 있습니다.

이러한 자료형은 기본형(primitive type)과 참조형(referece type)으로 나뉘는데,int 는 이 중 기본형에 속합니다.

기본형에는 다음과 같은 종류가 있습니다.

![https://velog.velcdn.com/images%2Fhadoyaji%2Fpost%2F238e3f45-1c32-49bf-98ff-ac2a2a4ba336%2Fjava_primitive_type.png](https://velog.velcdn.com/images%2Fhadoyaji%2Fpost%2F238e3f45-1c32-49bf-98ff-ac2a2a4ba336%2Fjava_primitive_type.png)

---

### 2) 그렇다면 Integer는 무엇인가? (wrapper class)

맨날 쓰던 Integer인데.... 어디에 썻더라..? 하고 생각해보면 주로

> ArrayList<Integer> intList = new ArrayList<Integer>();
	intList.add(1);
	intList.add(2);
	System.out.println(intList.get(0));
> 

> String stringNum = "123";
	int intNum = Integer.parseInt(stringNum);
	System.out.println(intNum);
> 

- Integer는 무엇인가 하면,1)에서 다룬 기본형을 표현해야 하는 경우가 있습니다.
- 매개변수로 객체를 필요로 할 때
- 기본형 값이 아닌 객체로 저장해야할 때
- 객체 간 비교가 필요할 때

이런 경우 **기본형을 객체로 다루기 위해 사용하는 클래스들을 래퍼 클래스(wrapper class)**라고 합니다.그리고 **Integer는 int의 레퍼클레스** 라고 할 수 있습니다.

모든 기본형은 래퍼클래스를 생성할 수 있고, 이는 아래와 같습니다.

![https://velog.velcdn.com/images%2Fhadoyaji%2Fpost%2F39b6ba49-ecc4-4886-a810-3923a0d07ebe%2F23233.jpg](https://velog.velcdn.com/images%2Fhadoyaji%2Fpost%2F39b6ba49-ecc4-4886-a810-3923a0d07ebe%2F23233.jpg)

---

**3) 그래서 int와 Integer는 어떻게 다른거지?**

int : 자료형(primitive type)

- 산술 연산 가능함
- null로 초기화 불가

Integer : 래퍼 클래스 (Wrapper class)

- Unboxing하지 않을 시 산술 연산 불가능함
- null값 처리 가능
- *boxing : primitive type -> wrapper class 변환 ( int to Integer )unboxing : wrapper class -> primitive type 변환 ( Integer to int )

으로 정리할 수 있을 것 같습니다.
