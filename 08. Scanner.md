### 화면에서 입력받기 - Scanner

#### Scanner란?
화면으로부터 데이터를 입력받는 기능을 제공하는 클래스  

#### Scanner를 사용하는 법

1) import문 추가  

import java.util.*;

2) Scanner 객체의 생성 

Scanner scanner = new Scanner(System.in - 화면 입력을 의미);

3) Scanner 객체를 사용  

int num =  Scanner.nextInt(); : 화면에서 입력받은 정수를 num에 저장  

String input = scanner.nextLine(한 행을 의미)(); : 화면에서 입력받은 내용을 input에 저장  
int num = Integer.parseInt(input); : 문자열(input)을 숫자(num)로 변환  
