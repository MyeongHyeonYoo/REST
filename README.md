# **Project - REST & Ajax**  ♻️

 ## 💡 `Spring` PROJECT <img src="https://img.shields.io/badge/Spring-5.0.7-darkgreen"> <img src="https://img.shields.io/badge/Java-11-purple"> <img src="https://img.shields.io/badge/JSP-2.1-orange"> <img src="https://img.shields.io/badge/Servlet-3.1-skyblue"> <img src="https://img.shields.io/badge/Tomcat-9.0.70-yellow"> <img src="https://img.shields.io/badge/Oracle-11.2.0.2.0-red">



---

### 🧾 프로젝트 소개 

---

>**ECLIPSE 환경 구축**

> 1. ECLIPSE 설치
> 2. JDK 설치
> 3. Oracle 설치 
> 4. Tomcat 설치

###### Eclipse Marketplace
> 5. Spring Tools 3 Add-On for Spring Tools 4 [3.9.22.RELEASE] 설치
> 6. Eclipse Enterprise Java and Web Developer Tools 3.20 설치
 
---

#### ◾ **START ▶ @GetMapping** 
- 환경설정 및 시작 - '안녕하세요' 확인<br>
<img src="img/rest_start(sample).jpg" width="400" height="150" style="border-radius: 5px;">
    - 타입 확인<br>
    <img src="img/type_text_plain.jpg" width="250" height="150" style="border-radius: 5px;">

<br>

#### ◾ **getSample** 
- 브라우저가 받은 데이터 - XML<br>
<img src="img/getSample.jpg" width="600" height="150" style="border-radius: 5px;">
    - 타입 확인<br>
    <img src="img/check_xml.jpg" width="250" height="150" style="border-radius: 5px;"><br>
      <img src="img/getSample2.jpg" width="600" height="150" style="border-radius: 5px;">

<br>

#### ◾ **getSample.json** 
- 브라우저가 받은 데이터 - JSON<br>
<img src="img/getSample.json.jpg" width="450" height="150" style="border-radius: 5px;">
    - 타입 확인<br>
    <img src="img/check_json.jpg" width="250" height="150" style="border-radius: 5px;">

<br>

#### ◾ **getList** 
- 브라우저가 받은 데이터 - XML<br>
<img src="img/getList.jpg" width="700" height="700" style="border-radius: 5px;">

<br>

#### ◾ **getList.json** 
- 브라우저가 받은 데이터 - JSON<br>
<img src="img/getList.json.jpg" width="300" height="700" style="border-radius: 5px;">

<br>

#### ◾ **getMap** 
- 브라우저가 받은 데이터 - XML<br>
<img src="img/getMap.jpg" width="600" height="150" style="border-radius: 5px;">

<br>

#### ◾ **getMap.json** 
- 브라우저가 받은 데이터 - JSON<br>
<img src="img/getMap.json.jpg" width="450" height="150" style="border-radius: 5px;">

<br>

#### ◾ **check** 
- 파라미터 값 주기<br>
<img src="img/check_height_weight.jpg" width="600" height="150" style="border-radius: 5px;"><br>
- General check - Status Code: 502<br>
    - height가 150 미만이면 HTTP상태메시지 전달<br>
<img src="img/check_bad_gateway(502).jpg" width="250" height="150" style="border-radius: 5px;"><br>

```
파라미터 값을 반드시 전달해 주어야 하고
하나라도 제대로 전달해 주지 않는다면,
'HTTP 상태 400 – 잘못된 요청' 에러 발생
```
     
<br>

#### ◾ **@PathVariable** 
<img src="img/atPathVariable.jpg" width="600" height="150" style="border-radius: 5px;"><br>
값을 얻을 때에는 int, double과 같은 기본 타입의 자료형은 사용 불가<br>
-> 포장 객체의 타입 ○

<br>

#### ◾ **REST방식의 테스트** 
#### ▶ @RunWith, @WebAppConfiguration, @ContextConfiguration, @Log4j
```
@RunWith(SpringJUnit4ClassRunner.class)

//Test for Controller
@WebAppConfiguration 
@ContextConfiguration({
	"file:src/main/webapp/WEB-INF/spring/root-context.xml",
	"file:src/main/webapp/WEB-INF/spring/appServlet/servlet-context.xml"
	})
@Log4j
```
#### ▶▶ @Before, @Test
- JUnit 기반의 테스트<br>
<img src="img/jUnit_test_testConvert.jpg" width="550" height="160" style="border-radius: 5px;"><br>
JSON 문자열이 Ticket타입의 객체로 변환
(코드 내의 Gson 라이브러리는 Java의 객체를 JSON 문자열로 변환하기 위해 사용)
    - test succes<br>
<img src="img/jUnit_test_testConvert_succes.jpg" width="200" height="150" style="border-radius: 5px;"><br>
JUnit을 이용하는 방식의 테스트 장점은 Tomcat을 구동하지 않고도 컨트롤러를 구동해 볼 수 있다.
```
↘ 크롬 확장 프로그램 (REST 방식 테스트 도구)
Chrome 브라우저 앱스토어(chrome://apps/) -> 'REST client' 검색
curl(https://curl.haxx.se/) -> 리눅스, Mac 전용

```
#### ◾ 크롬 확장 프로그램 'Yet Another REST Client' 사용하여 테스트
<img src="img/Yet_Another_REST_Client_TEST_1.jpg" width="600" height="500" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_1_2.jpg" width="600" height="200" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_2.jpg" width="600" height="400" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_3.jpg" width="600" height="400" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_4.jpg" width="600" height="400" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_5.jpg" width="600" height="400" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_5.jpg" width="600" height="400" style="border-radius: 5px;"><br>

##### 콘솔 출력 화면
<img src="img/Yet_Another_REST_Client_TEST_console.jpg" width="600" height="100" style="border-radius: 5px;"><br>

※ **톰캣 서버 실행하지 않으면** `POST`방식으로 전송할 수 없어 **'ERROR'** 발생<br>
<img src="img/Yet_Another_REST_Client_TEST_ERROR.jpg" width="600" height="180" style="border-radius: 25px;">

---



```

```

