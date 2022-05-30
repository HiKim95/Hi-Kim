### 자동 형변환

작은 타입의 값을 큰 타입의 변수에 저장할 경우 컴파일러가 자동으로 형변환함   
ex)  
float f = 1234;  
자동→ float f = (float)1234;   

반대로 큰 타입의 값을 작은 타입의 변수에 저장할 경우 에러가  
발생하기 때문에 수동으로 형변환을 시켜줘야함
ex)  
int i = 3.14f; → 에러  
int i = (int)3.14f; → 작동(값 손실 발생)  

|종류|크기||
|--|--|--|
|byte|1byte|↓|
|short,char|2byte|↓|
|int|4byte|↓|
|long|8byte|↓|
|float|4byte|↓|
|double|8byte|| 

long과 float 타입의 경우 크기 자체는 long이 8byte로 크지만   
실제로는 정수형인 long보다 실수형인 float가 표현하는 값의 범위가 크기 때문에 가능함  

예외로 큰 타입의 값일지라도 작은 타입의 변수의 범위 내라면 자동 형변환됨   
ex)  
byte b = 100;  
자동→ byte b = (byte)100;  

다만 범위 내의 값이라도 큰 타입의 변수에 저장된 값이면 자동 형변환 하지않음  
ex)  
int i = 100;
byte b = i; → 에러  
byte b = (btye)i; → 동작
