<h1 align="center">🚑<strong> findER - Refactoring </strong>🚑</h1>

<div align="center">
  <strong>2023년 제17회 공개 SW 개발자대회</strong>
  <br><br>
  <em>실시간 응급실 정보 제공 애플리케이션, findER(Emergency Room)</em>
  <br><br>
  <em>written by gretea5 & wingunkh</em>
</div>

<div align="center">
    <h3>
    <a href="https://malalove.notion.site/API-2f5e86d852ca4f73b2e66c21b8a31e3d?pvs=4">
      📜 REST API 명세서
    </a>
    <span> | </span>
    <a href="https://github.com/gretea5/findER">
      🖼️ Frontend
    </a>
  </h3>
</div>

<br>

## 📑 목차
- ✍🏻 **프로젝트 개요**
- ⭐ **주요 기능**
- 📚 **기술 스택**
- 🗺️ **시스템 구조도**
- 👩‍👩‍👧‍👦 **팀원 및 담당 파트**
- 🛠️ **리팩터링**

<br>

## ✍🏻 프로젝트 개요
'응급실 뺑뺑이'란 응급 환자가 이송 병원을 정하지 못해 다른 병원에 재이송되는 현상을 의미합니다. <br><br>
이러한 현상으로 인해 환자가 사망에 이르는 사회적 문제가 나날이 대두되고 있습니다. <br><br>
저희 팀은 '응급실에 대한 정보 부족'이 해결될 수 있다면 이러한 문제가 줄어들 것으로 판단하여 <br>
실시간 응급실 정보 제공 서비스 애플리케이션을 개발하게 되었습니다. <br><br>
애플리케이션의 이름은 응급실(Emergency Room)을 찾는(find) 매개체라는 의미에서 ‘findER’로 선정하였습니다. <br><br>
해당 애플리케이션을 사용하는 사용자는 응급 상황 발생 시 자신의 위치를 기준으로 가까운 순서대로 <br>
응급실의 위치, 예상 도착 시간, 최적 경로 등을 확인할 수 있습니다. <br><br>
또한 각 응급실의 잔여 병상 수를 실시간으로 확인 가능함과 동시에 현재 시각으로부터 2시간 동안의<br>
병상 이용 가능 시간 비율 및 병상 수 변동 추이 그래프를 제공하여 사용자가 최적의 응급실을 선택하는 데 있어 도움을 줄 수 있습니다.

<br>

## ⭐ 주요 기능
blank

<br>

## 📚 기술 스택
<div>
    <table>
        <tr>
            <td colspan="2" align="center">
                Language
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white"> 
                <img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=openjdk&logoColor=white">
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                Framework
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
                <img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                API
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/DATA.go.kr-00529B?style=for-the-badge&logo=D&logoColor=white"> 
                <img src="https://img.shields.io/badge/Kakao Map-FFCD00?style=for-the-badge&logo=kakao&logoColor=black"> 
                <img src="https://img.shields.io/badge/Kakao Mobility-FFCD00?style=for-the-badge&logo=kakao&logoColor=black">
                <img src="https://img.shields.io/badge/Kakao Local-FFCD00?style=for-the-badge&logo=kakao&logoColor=black"> 
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
                <img src="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
                <img src="https://img.shields.io/badge/oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white">
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                Tool
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/Android Studio-3DDC84?style=for-the-badge&logo=androidstudio&logoColor=white">
                <img src="https://img.shields.io/badge/IntelliJ IDEA-000000?style=for-the-badge&logo=intellijidea&logoColor=white">
            </td>
        </tr>
        <tr>
            <td colspan="2" align="center">
                etc.
            </td>
            <td colspan="4">
                <img src="https://img.shields.io/badge/postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white">
                <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white">
            </td>
        </tr>
    </table>
</div>

<br>

## 🗺️ 시스템 구조도
blank

<br>

## 👩‍👩‍👧‍👦 팀원 및 담당 파트
<table>
  <tr>
    <td colspan="1" align="center"><strong>Front-End</strong></td>
    <td colspan="1" align="center"><strong>Back-End</strong></td>
  </tr>
  
  <tr>
    <td align="center">
        <img src="https://avatars.githubusercontent.com/u/120379834?v=4" width="150px;" alt="박장훈"/>
    </td>
    <td align="center">
        <img src="https://avatars.githubusercontent.com/u/58140360?v=4" width="150px" alt="김현근"/>
    </td>
  </tr>

  <tr>
    <td colspan="1" align="center">
      <a href="https://github.com/gretea5"><strong>박장훈</strong></a>
    </td>
    <td colspan="1" align="center">
      <a href="https://github.com/wingunkh"><strong>김현근</strong></a>
    </td>
  </tr>

  <tr>
    <td colspan="1" align="center"><strong>Android Mobile Application 개발 (Kotlin)</strong></td>
    <td colspan="1" align="center"><strong>Spring Web Application 개발 (Java)</strong></td>
  </tr>
</table>

<br>

## 🛠️ 리팩터링
blank
