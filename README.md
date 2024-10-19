# java-calculator-precourse

## 기능 요구사항

- [ ] 사용자 입력 받기
    - [ ] 사용자는 숫자와 구분자(`,` , `:`, `커스텀 구분자`)로 이루어진 문자열을 입력한다.
        - 구분자는 혼용해서 사용 가능하고 한 가지만 사용해도 된다.
    - 예시 :
        - ""
        - "1,2"
        - "1,2,3"
        - "1,2:3"
    - `커스텀 구분자`는 `//`와 `\n` 사이에 위치하는 문자이다.
        - [x] `커스텀 구분자`는 문자열의 맨 앞부분에 와야한다.
        - [x] `커스텀 구분자`는 하나만 허용한다.
        - 예시 :
            - "//;\n1;2;3"
        -[x] `커스텀 구분자`는 한 글자만 가능하고, 숫자가 될 수 없다. 기본 구분자도 `커스텀 구분자`로 입력될 수 있다.
            - 가능한 예시 :
                - "//a\n1a2a3"
                - "//-\n1-2-3"
            - 불가능한 예시 :
                - "//1\n11213"
                - "//aa\n1aa2aa3"
    -[ ] 구분자의 앞뒤에는 숫자가 있어야 한다.
        - 불가능한 예시 :
            - "1,"
    -[ ] 그 외 다른 문자가 들어오면 예외 처리한다.
        - 불가능한 예시 :
            - "a,bc"

- [ ] 더하기
    - 구분자로 분리된 숫자들을 더한다.
- [ ] 출력
    - 덧셈결과를 아래와 같이 출력한다.
    - 예시 :
        - 결과 : 6