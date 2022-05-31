### 조건문과 반복문

조건문(if, switch) : 조건을 만족할때만 {}를 수행 (0 ~ 1번)   

반복문(for, while) : 조건을 만족하는 동안 {}를 수행 (0 ~ n번)    

두개를 합쳐서 제어문(flow control statement) 이라함   

#### if문

조건식이 참(true)일 때, 괄호{}안의 문장들을 수행한다.  

if (조건식);  
  
#### if-else문

둘 중의 하나 - 조건식이 참일 때와 거짓일 때로 나눠서 처리   

if (조건식);{
} else{
};  

#### 중첩 if문 - if문 안의 if

앞의 if문을 처리한 뒤 안의 if문을 처리함   
if (조건식 1);{   
if(조건식 2);{  
} else if(조건식 3){   
};   
} else {   
};     

#### switch문

처리해야 하는 경우의 수가 많을 때 유용한 조건문  

switch(조건){  
case 조건1 : 동작 break; - break를 사용하지 않을 시 default도 동작  
case 조건2 : 동작 break;   
default : 동작 break;  
}  

##### switch문의 제약 조건

1. switch문의 저건식 결과는 정수 또는 문자열이어야함
2. case문의 값음 정수, 상수(문자 포함), 문자열만 가능하며, 중복되지 않아야함  

제약 조건때문에 사용하지 못할 경우엔 if,else if문을 사용해야함  

#### 임의의 정수(난수) 만들기

Math.random() - 0.0 과 1.0 사이의 double 값을 반환  
0.0 <= Math.random() < 1.0  

