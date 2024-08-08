<h1 align="center">🍄<strong> MapleStory Chatbot </strong>🍄</h1>

<div align="center">
  <em>메이플스토리의 다양한 최신 소식을 간편하게 확인할 수 있는 카카오톡 챗봇</em>
  <br><br>
</div>

<br>

## Description
- 스마트폰으로 메이플스토리 소식을 확인하려면 메이플스토리 공식 사이트에 접속한 후, 뉴스 섹션을 클릭하고, 원하는 섹션을 클릭하고, 원하는 소식을 클릭해야 하는 번거로운 과정이 필요합니다. <br>
- 또한 공식 사이트가 모바일 버전 최적화가 되어 있지 않아 불편함이 더욱 크다고 느꼈습니다. <br>
- 이를 개선하고자 NEXON Open API를 활용하여 공지사항 등 메이플스토리의 다양한 최신 정보를 간편하게 확인할 수 있는 카카오톡 챗봇을 개발했습니다.

<br>

## Architecture
<img width="600" height="360" src="https://github.com/user-attachments/assets/ba6f2e26-4d5e-4c6e-ae07-69039067219b"> <br>

<br>

## Tech Stack
<div>
    <table>
        <tr>
            <td colspan="2" align="center">
                Language
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=openjdk&logoColor=white">
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                Framework
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
                <img src="https://img.shields.io/badge/Spring Batch-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                API
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/NEXON Open API-0054A3?style=for-the-badge&logo=nginx&logoColor=white"> 
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                Server
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/amazon ec2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white"> 
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                Database
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/Amazon RDS-527FFF?style=for-the-badge&logo=Amazon RDS&logoColor=white">
                <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=white">
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                Tool
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/IntelliJ IDEA-000000?style=for-the-badge&logo=intellijidea&logoColor=white">
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                etc.
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/KakaoTalk-FFCD00?style=for-the-badge&logo=KakaoTalk&logoColor=black">
                <img src="https://img.shields.io/badge/FileZilla-BF0000?style=for-the-badge&logo=FileZilla&logoColor=white">
                <img src="https://img.shields.io/badge/postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white">
            </td>
        </tr>
    </table>
</div>

<br>

## Screenshots

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/0d3dc0fb-926a-46ca-be33-3d2d981cb405" width="300" height="650"><p>기본 메시지</p></td>
    <td><img src="https://github.com/user-attachments/assets/2d886a51-4539-4dca-9fe9-2cd5bfc72ab8" width="300" height="650"><p>공지사항 확인 기능</p></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/9127ea62-2f9d-46a1-aaa1-95b1bf7df429" width="300" height="650"><p>클라이언트 업데이트 확인 기능</p></td>
    <td><img src="https://github.com/user-attachments/assets/5656461d-4fb5-424f-beaa-e0d49feff65a" width="300" height="650"><p>진행 중 이벤트 확인 기능</p></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/6353e7a0-0a54-44f0-8eb9-7f92c2a8dc74" width="300" height="650"><p>캐시샵 공지 확인 기능</p></td>
  </tr>
</table>

<br>

## How it works?
1. 서버는 최초 실행 시 NEXON Open API를 호출하여 공지사항, 클라이언트 업데이트, 진행 중 이벤트, 캐시샵 공지 데이터를 요청합니다.
2. 데이터를 Amazon RDS DB (MySQL)에 저장합니다.
3. 카카오톡 챗봇의 요청에 해당하는 데이터를 JSON 형식으로 응답합니다. <br>
   (Spring Cache & ehcache 3에 의해 당일 최초 요청 데이터가 아닐 경우 DB를 거치지 않습니다.)
4. 매일 오전 03:00에 NEXON Open API를 호출하여 데이터를 갱신합니다. <br>
   (Spring Batch에 의해 갱신 과정은 비동기 병렬 처리됩니다.)

<br>
