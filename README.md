<h1 align="center">🚑<strong> findER - Refactoring </strong>🚑</h1>

<div align="center">
  <strong>2023년 제17회 공개 SW 개발자대회</strong>
  <br><br>
  <em>실시간 응급실 정보 제공 애플리케이션, findER(Emergency Room)</em>
  <br><br>
  <em>written by wingunkh</em>
</div>

<div align="center">
  <h3>
    <!--
    <a href="https://malalove.notion.site/API-2f5e86d852ca4f73b2e66c21b8a31e3d?pvs=4">
      📜 REST API 명세서
    </a>
    <span> | </span>
    -->
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
응급실 병상이 없어서 환자가 떠돌다가 숨지는, 이른바 **'응급실 뺑뺑이'** 현상이 사회적 이슈로 부각되고 있습니다.
<br>
이에 저희 팀은 이러한 사회적 문제를 해결하는 데 일조하고자 **실시간 잔여 병상 수를 포함한 다양한 응급실 관련 정보를 제공하는 애플리케이션**을 개발하였습니다.
<br>
<br>
📰 [<ins>'응급실 뺑뺑이' 잇단 사망‥왜 반복되나</ins> (MBC 뉴스)](https://imnews.imbc.com/replay/2023/nwtoday/article/6488902_36207.html)

<br>

## ⭐ 주요 기능
> ### 응급실 정보 제공 (위치, 전화번호 外 CT & MRI 촬영 가능 여부 등)
<details>
  <summary><b>화면 보기</b></summary>
  <br>
  <img 
    width="325"
    height="720"
    src="https://github-production-user-asset-6210df.s3.amazonaws.com/120379834/281963820-c3d78076-d0bc-49bb-8d50-1fdbe855fb8f.png">
  <br><br>
</details>

> ### 응급실 잔여 병상 수 실시간 제공 (1분 간격 갱신)
<details>
  <summary><b>화면 보기</b></summary>
  <br>
  <img 
    width="325" 
    height="720"
    src="https://github.com/gretea5/findER-frontend/assets/120379834/e685a776-cbbc-4e65-8f90-36dfc40df6bc">
  <br><br>
</details>

> ### 카카오 맵 API를 통한 사용자 현재 위치 기준 가까운 응급실 목록 및 최적 경로 제공
<details>
  <summary><b>화면 보기</b></summary>
  <br>
  <img 
    width="325" 
    height="720" 
    src="https://github.com/gretea5/findER-frontend/assets/120379834/633431e6-621b-4ddf-acb0-aa9e47d6e7a8">
  <br><br>
</details>


> ### 카카오 모빌리티 API를 통한 응급실 예상 도착 시간 및 이동 거리 제공
<details>
  <summary><b>화면 보기</b></summary>
  <br>
  <img 
    width="325" 
    height="720" 
    src="https://github.com/gretea5/findER-frontend/assets/120379834/6a974298-75fa-4514-a69e-029b8fe2fff8">
  <br><br>
</details>

> ### 사용자 문진표 작성 기능 제공
<details>
  <summary><b>화면 보기</b></summary>
  <br>
  <img 
    width="325" 
    height="720" 
    src="https://github.com/gretea5/findER-frontend/assets/120379834/c9653656-5634-42e9-91b7-99d5032d7f6e">
  <br><br>
</details>

> ### 사용자 간 문진표 연동을 통한 문진표 상호 동기화 기능 제공
<details>
  <summary><b>화면 보기</b></summary>
  <br>
  <img 
    width="325"
    height="720"
    src="https://github.com/gretea5/findER-frontend/assets/120379834/e76a8915-4b0a-4197-80ae-1c578dd3c059">
  <br><br>
</details>

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

<img width="600" alt="image" src="https://github.com/wingunkh/tmp/assets/58140360/78e17e49-3ae2-46d3-bf9d-1396d6741f09">

<br>

## 👩‍👩‍👧‍👦 팀원 및 담당 파트

<table>
  <tr>
    <td align="center">Front-End</td>
    <td align="center">Back-End</td>
  </tr>
  
  <tr>
    <td align="center">
        <img src="https://avatars.githubusercontent.com/u/120379834?v=4" width="120px;" alt="박장훈"/>
    </td>
    <td align="center">
        <img src="https://avatars.githubusercontent.com/u/58140360?v=4" width="120px" alt="김현근"/>
    </td>
  </tr>

  <tr>
    <td align="center">
      <a href="https://github.com/gretea5">박장훈</a>
    </td>
    <td align="center">
      <a href="https://github.com/wingunkh">김현근</a>
    </td>
  </tr>

  <tr>
    <td align="center" width="50%">Android Mobile Application 개발 (Kotlin)</td>
    <td align="center" width="50%">Spring Web Application 개발 (Java)</td>
  </tr>
</table>

<br>

<!-- ## 🛠️ 리팩터링
blank
-->
