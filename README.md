# Wemakeprice 1차 과제
> URL 파싱 후 데이터 가공 출력

## 개발 프레임워크 및 라이브러리
* Java 1.8
* Spring Boot 2.2.7
* Gradle
* Lombok
* Jsnoup
* thymeleaf

## 제약 조건
1. 모든 문자 입력
   - 세상에 존재하는 모든 형태의 URL을 입력받는다.
2. 영어, 숫자 출력
   - 결과 데이터는 영어와 숫자로만 구성된 데이터만 출력한다  
     > 노출 유형이 HTML 일 경우는 `<>` 형식의 HTML TAG 를 제거하고 출력한다  
       노출 유형이 TEXT 일 경우에는 모든 영어와 숫자로만 구성된 데이터를 출력한다 
3. 오름차순
   - 영어 : AaBbCcDd `...` Zz
   - 숫자 : 0123456789
5. 교차 출력
   - 영어 숫자 영어 숫자 `...`  
     > 더 이상 출력될 숫자 또는 영어가 없을 경우 남아있는 정렬된 문자열 그대로 출력
6. 출력 묶음 단위
   - 사용자가 입력한 자연수의 묶음 단위를 기준으로 몫과 나머지를 구하여 노출
   
## 빌드 및 실행방법
- `gradle build && java -jar build/libs/wemakeprice_parsetest-0.0.1.jar`
- [http://localhost:8080](http://localhost:8080) 접속 후 기능 테스트