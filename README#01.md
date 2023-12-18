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








