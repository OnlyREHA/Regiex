### 정규표현식

/regiex/  --> Regular expression의 약자

#### 언제사용하는가?
- 텍스트에서 우리가 원하는 특정한 패턴을 찾을 때 (전화번호형태의 패턴, 웹사이츠주소형태의 패턴, 이메일형식의 패턴 등등)
- 사용자가 입력한 텍스트가 이메일이나 패스워드와 같이 특정한 패턴에 부합하는지 유효성 검사를 할때도 사용할수 있다.
- 정규식은 문자를 검사하고자 할때 사용하는 식이다.

#### 정규식은 /로 시작하여 "나는 정규표현식"임을 나타낸다.
- /우리가 찾고자하는 패턴/
- /regiex/i

-i는 어떤 옵션에 따라 검색할껀지 플래그를 활용할수 있다.

#### 문법
1) Groups anf ranges

- | : 또는
   
![image](https://github.com/OnlyREHA/Regiex/assets/145514740/cf6466bd-d9ed-4f67-b3be-56173b1de357)
     
- () : 그룹
   
![image](https://github.com/OnlyREHA/Regiex/assets/145514740/47c285c8-3419-4bc7-8d1b-be7607f81fb6)

- [] : 문자셋, 괄호안의 어떤 문자든

![image](https://github.com/OnlyREHA/Regiex/assets/145514740/385b5fa9-5edd-48cc-83d9-13d4aa11af39)

대괄호 안에 있는 글자중 하나라도 만족하는 것을 찾아라는 의미

     
- [^] : 부정문자셋, 괄호안의 어떤 문자가 아닐때
  
     
- (?) : 찾지만 기억하지는 않음
    
![image](https://github.com/OnlyREHA/Regiex/assets/145514740/9b1cc86e-9965-4b33-a544-8dfd04b3254f)


#### 아래 두이미지는 gr로 시작해서 a~g

![image](https://github.com/OnlyREHA/Regiex/assets/145514740/edc9d9eb-0a4c-4973-b00c-6dda00976332)  ![image](https://github.com/OnlyREHA/Regiex/assets/145514740/e3d32fea-e8c3-48b3-9a0f-e501bd0fb1c7)


2) 제한하기위해 사용하는
- ? :없거나 있거나(zero or one)
- : 없거나 있거나 많거나(zero or more)
- : 하나 또는 많거나(one or more)
- {n} : n번 반복
- {min,} : 최소
- {min,max} : 최소 그리고 최대

  
 3) 경계에 대한
- \b : 단어경계
-> Ya로 시작하는 단어

![image](https://github.com/OnlyREHA/Regiex/assets/145514740/a4d2a238-2fcb-489c-8039-45269c1d1b47)

-> Ya로 끝나는 단어 
![image](https://github.com/OnlyREHA/Regiex/assets/145514740/f60f0b22-bb3e-4f38-8f1c-8c920a2f0b2f)

- \B : 단어경계가 아님
  
- ^ : 문장의 시작

-> 문장의 시작인 Ya

![image](https://github.com/OnlyREHA/Regiex/assets/145514740/2e6c7515-f644-471d-a678-bfd794b2c939)

- $ : 문장의 끝

-> 문장의 긑인 Ya

![image](https://github.com/OnlyREHA/Regiex/assets/145514740/4be53c66-9a7c-40fe-b772-95e0dd8b9266)


4) 특징을 이용하는 방법
- \ : 특수문자가 아닌 문자
- . : 어떤 글자(줄바꿈 문자 제외)

-> 문장의 모든 문자

![image](https://github.com/OnlyREHA/Regiex/assets/145514740/00756107-1538-4e70-bfc6-549209c3204d)

- \d: 숫자
- \D: 숫자 아님
- \w : 문자
- \W : 문자 아님
- \s : 공백
- \S : 공백 아님








