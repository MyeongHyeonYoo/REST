# **Project - REST & Ajax**  โป๏ธ

 ## ๐ก `Spring` PROJECT <img src="https://img.shields.io/badge/Spring-5.0.7-darkgreen"> <img src="https://img.shields.io/badge/Java-11-purple"> <img src="https://img.shields.io/badge/JSP-2.1-orange"> <img src="https://img.shields.io/badge/Servlet-3.1-skyblue"> <img src="https://img.shields.io/badge/Tomcat-9.0.70-yellow"> <img src="https://img.shields.io/badge/Oracle-11.2.0.2.0-red">



---

### ๐งพ ํ๋ก์ ํธ ์๊ฐ 

---

>**ECLIPSE ํ๊ฒฝ ๊ตฌ์ถ**

> 1. ECLIPSE ์ค์น
> 2. JDK ์ค์น
> 3. Oracle ์ค์น 
> 4. Tomcat ์ค์น

###### Eclipse Marketplace
> 5. Spring Tools 3 Add-On for Spring Tools 4 [3.9.22.RELEASE] ์ค์น
> 6. Eclipse Enterprise Java and Web Developer Tools 3.20 ์ค์น
 
---

### REST ๋ฐฉ์์ ์ ํ

#### โพ **START โถ @GetMapping** 
- ํ๊ฒฝ์ค์  ๋ฐ ์์ - '์๋ํ์ธ์' ํ์ธ<br>
<img src="img/rest_start(sample).jpg" width="400" height="150" style="border-radius: 5px;">
    - ํ์ ํ์ธ<br>
    <img src="img/type_text_plain.jpg" width="250" height="150" style="border-radius: 5px;">

<br>

#### โพ **getSample** 
- ๋ธ๋ผ์ฐ์ ๊ฐ ๋ฐ์ ๋ฐ์ดํฐ - XML<br>
<img src="img/getSample.jpg" width="600" height="150" style="border-radius: 5px;">
    - ํ์ ํ์ธ<br>
    <img src="img/check_xml.jpg" width="250" height="150" style="border-radius: 5px;"><br>
      <img src="img/getSample2.jpg" width="600" height="150" style="border-radius: 5px;">

<br>

#### โพ **getSample.json** 
- ๋ธ๋ผ์ฐ์ ๊ฐ ๋ฐ์ ๋ฐ์ดํฐ - JSON<br>
<img src="img/getSample.json.jpg" width="450" height="150" style="border-radius: 5px;">
    - ํ์ ํ์ธ<br>
    <img src="img/check_json.jpg" width="250" height="150" style="border-radius: 5px;">

<br>

#### โพ **getList** 
- ๋ธ๋ผ์ฐ์ ๊ฐ ๋ฐ์ ๋ฐ์ดํฐ - XML<br>
<img src="img/getList.jpg" width="700" height="700" style="border-radius: 5px;">

<br>

#### โพ **getList.json** 
- ๋ธ๋ผ์ฐ์ ๊ฐ ๋ฐ์ ๋ฐ์ดํฐ - JSON<br>
<img src="img/getList.json.jpg" width="300" height="700" style="border-radius: 5px;">

<br>

#### โพ **getMap** 
- ๋ธ๋ผ์ฐ์ ๊ฐ ๋ฐ์ ๋ฐ์ดํฐ - XML<br>
<img src="img/getMap.jpg" width="600" height="150" style="border-radius: 5px;">

<br>

#### โพ **getMap.json** 
- ๋ธ๋ผ์ฐ์ ๊ฐ ๋ฐ์ ๋ฐ์ดํฐ - JSON<br>
<img src="img/getMap.json.jpg" width="450" height="150" style="border-radius: 5px;">

<br>

#### โพ **check** 
- ํ๋ผ๋ฏธํฐ ๊ฐ ์ฃผ๊ธฐ<br>
<img src="img/check_height_weight.jpg" width="600" height="150" style="border-radius: 5px;"><br>
- General check - Status Code: 502<br>
    - height๊ฐ 150 ๋ฏธ๋ง์ด๋ฉด HTTP์ํ๋ฉ์์ง ์ ๋ฌ<br>
<img src="img/check_bad_gateway(502).jpg" width="250" height="150" style="border-radius: 5px;"><br>

```
ํ๋ผ๋ฏธํฐ ๊ฐ์ ๋ฐ๋์ ์ ๋ฌํด ์ฃผ์ด์ผ ํ๊ณ 
ํ๋๋ผ๋ ์ ๋๋ก ์ ๋ฌํด ์ฃผ์ง ์๋๋ค๋ฉด,
'HTTP ์ํ 400 โ ์๋ชป๋ ์์ฒญ' ์๋ฌ ๋ฐ์
```
     
<br>

#### โพ **@PathVariable** 
<img src="img/atPathVariable.jpg" width="600" height="150" style="border-radius: 5px;"><br>
๊ฐ์ ์ป์ ๋์๋ int, double๊ณผ ๊ฐ์ ๊ธฐ๋ณธ ํ์์ ์๋ฃํ์ ์ฌ์ฉ ๋ถ๊ฐ<br>
-> ํฌ์ฅ ๊ฐ์ฒด์ ํ์ โ

<br>

#### โพ **REST๋ฐฉ์์ ํ์คํธ** 
#### โถ @RunWith, @WebAppConfiguration, @ContextConfiguration, @Log4j
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
#### โถโถ @Before, @Test
- JUnit ๊ธฐ๋ฐ์ ํ์คํธ<br>
<img src="img/jUnit_test_testConvert.jpg" width="550" height="160" style="border-radius: 5px;"><br>
JSON ๋ฌธ์์ด์ด Ticketํ์์ ๊ฐ์ฒด๋ก ๋ณํ
(์ฝ๋ ๋ด์ Gson ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ Java์ ๊ฐ์ฒด๋ฅผ JSON ๋ฌธ์์ด๋ก ๋ณํํ๊ธฐ ์ํด ์ฌ์ฉ)
    - test succes<br>
<img src="img/jUnit_test_testConvert_succes.jpg" width="200" height="150" style="border-radius: 5px;"><br>
JUnit์ ์ด์ฉํ๋ ๋ฐฉ์์ ํ์คํธ ์ฅ์ ์ Tomcat์ ๊ตฌ๋ํ์ง ์๊ณ ๋ ์ปจํธ๋กค๋ฌ๋ฅผ ๊ตฌ๋ํด ๋ณผ ์ ์๋ค.
```
โ ํฌ๋กฌ ํ์ฅ ํ๋ก๊ทธ๋จ (REST ๋ฐฉ์ ํ์คํธ ๋๊ตฌ)
Chrome ๋ธ๋ผ์ฐ์  ์ฑ์คํ ์ด(chrome://apps/) -> 'REST client' ๊ฒ์
curl(https://curl.haxx.se/) -> ๋ฆฌ๋์ค, Mac ์ ์ฉ

```
#### โพ ํฌ๋กฌ ํ์ฅ ํ๋ก๊ทธ๋จ 'Yet Another REST Client' ์ฌ์ฉํ์ฌ ํ์คํธ
<img src="img/Yet_Another_REST_Client_TEST_1.jpg" width="600" height="500" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_1_2.jpg" width="600" height="200" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_2.jpg" width="600" height="400" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_3.jpg" width="600" height="400" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_4.jpg" width="600" height="400" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_5.jpg" width="600" height="400" style="border-radius: 5px;"><br>
<img src="img/Yet_Another_REST_Client_TEST_5.jpg" width="600" height="400" style="border-radius: 5px;"><br>

##### ์ฝ์ ์ถ๋ ฅ ํ๋ฉด
<img src="img/Yet_Another_REST_Client_TEST_console.jpg" width="600" height="100" style="border-radius: 5px;"><br>

โป **ํฐ์บฃ ์๋ฒ ์คํํ์ง ์์ผ๋ฉด** `POST`๋ฐฉ์์ผ๋ก ์ ์กํ  ์ ์์ด **'ERROR'** ๋ฐ์<br>
<img src="img/Yet_Another_REST_Client_TEST_ERROR.jpg" width="600" height="180" style="border-radius: 25px;">

---



```

```

