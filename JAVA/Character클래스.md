## 🪄Character 클래스
# - 문자 데이터에 대한 다양한 처리를 위한 상수 및 메서드 제공 

 char ch = 'A';
System.out.println("ch = " + ch) 

isXXX() 메서드 : 특정 대상인지 여부 판별
ch 는 대문자인가? " + Character.isUpperCase(ch)
ch 는 소문자인가? " + Character.isLowerCase(ch)
"ch 는 문자인가? " + Character.isLetter(ch)
"ch 는 숫자인가? " + Character.isDigit(ch)
"ch 는 공백문자인가? " + Character.isWhitespace(ch)
"ch 는 공백문자인가? " + Character.isSpace(ch)
=> Deprecated 로 표시되는 메서드. 사용 가능하나
isWhilespace() 메서드로 대체됨
