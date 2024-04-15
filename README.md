# 전자결재
<br>

## 📗 목차

<b>
  
- 📝 [개요](#-개요)
- 🛠 [기술 및 도구](#-기술-및-도구)
- 👨🏻‍💻 [기능 구현](#-기능-구현)
- 💾 [업데이트](#-업데이트)
- ⭐️ [PowerAutomate 로직](#%EF%B8%8F-powerautomate-로직)
- 💎 [DB 정보](#-DB-정보)
- 🚀 [배포](#-배포)
- 🔗 [참고자료](#-참고자료)

</b>

<br>

## **📝 개요**
<br>![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/56588de0-1e8f-492f-8d02-8b19e66b24f9)

> **프로젝트**: 전자결재
>
> **기획 및 제작**: 최준범
>
> **분류**: 개인 프로젝트
>
> **제작 기간**: 2023.12.14. ~ 
>
> **배포일**: 2024.01.24
>
> **사용 기술**: Python, Flask, MSSQL, Azure, PowerAutomate, HTML5, CSS3, JavaScript
>
> **문의**: junbeom.choi@radiantgrace.org

<br />

## **🛠 기술 및 도구**

<img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=Python&logoColor=white"> <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white"> 
<img src="https://img.shields.io/badge/MSSQL-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white"> <img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/powerautomate-0066FF?style=for-the-badge&logo=powerautomate&logoColor=white">
<br>
<img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> <img src="https://img.shields.io/badge/css3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white">


<br />

## **👨🏻‍💻 기능 구현**

### 1. 로그인 페이지 구현
<br>

![login](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/4240e2aa-5f17-4664-8c69-7b529bbb8f02)<br/>

- 기존에 사용하던 Office 365 계정과 동일한 계정으로 로그인

<br/>

### 2. 문서결재 요청 구현
<br>

![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/a140b288-552d-4c43-9191-202b9c2e844f)<br/>

- 가장 기본적인 기안 양식을 HTML로 구현
<br/>

  ### 2-1. DatePicker 사용으로 날짜선택<br>
  <details>
  <summary> DatePicker </summary>

  ![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/90494b23-702c-496b-acb0-e4d8115df155)<br/>

  - Bootstrap 기능인 DatePicker 사용
  </details><br>

  ### 2-2. 결재선 지정 기능<br>
  <details>
  <summary> 결재선 </summary>
    
  ![orgtree](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/85240574-dc0e-4169-910b-885e5715a24b)<br/>

  - <결재선 지정> 버튼 클릭 시 새창으로 결재선 지정 창 구현
  - 결재선 지정 시, 각각 결재자, 참조자 이름 문서에 자동 기입 구현
  - 결재선 지정 시, '제출'버튼 visible 구현
  </details><br/>

  ### 2-3. 파일 업로드<br>
  <details>
  <summary> 파일 업로드 </summary>

  ![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/c61df01d-d058-460a-8cb0-bb2ba001e0d2)<br/>

  - 로컬 파일을 업로드하여 첨부파일 기능 구현
  - 여러개의 파일 동시에 업로드 기능 구현
  </details><br>

### 3. 메신저 알림 구현 (MS Teams)
<details>
<summary> 기존 알림 구현 </summary>

<br>
  
![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/fcaacf44-91ab-4730-a0b1-1311bf7bb12c)![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/97ccc755-31fe-4529-b59e-a3cde0896e8e)<br/>

- 사내 메신저 (MS Teams)로 결재진행 및 참조 알림 기능 구현

</details>

<br>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/5d650380-cdc1-42ad-a265-452a5df721cb)

<br>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/6a0ad7cb-7373-430c-8666-89fa84ca7196)

- 흐름봇을 통한 결재사항 및 URL 알림 구현
- 전자결재 앱의 문서 Detail 에서 승인 및 반려 처리 구현



<br>

### 4. 결재 문서 열람
<br>

![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/bee1fd97-3034-4d58-b1b7-c6b5c3aec9de)<br/>

- 기안자 열 값이 현재 로그인 중인 유저의 계정 값과 일치하는 문서들만 출력
<br>

### 4-1. 문서 상세보기<br>
<details>
<summary> 문서 상세보기 </summary>

![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/e5f56e31-95a6-4519-9c52-91156a9ceab0)<br/>

- 작성된 문서 열람 및 결재 진행 상황 확인 가능
</details><br>

### 4-2. 프린트<br>
<details>
<summary> 프린트 </summary>

![print](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/c4a7fc70-cf20-45a6-8222-1ca44e944349)<br/>

- 프린트 버튼으로 필요한 양식만 출력 기능 구현
</details><br>

### 4-3. 첨부파일<br>
<details>
<summary> 첨부파일 </summary>

![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/7ecb5e39-1b13-4bd1-99d1-2ad0381319ea)<br/>

- 문서 하단 업로드된 첨부파일 열기 || 저장 기능 구현
</details><br>

## **💾 업데이트**

### 24-01-25 업데이트
<details>
<summary> 자세히 보기 </summary>
  
- ### 문서번호 자동생성 및 적용
  
예) CJH-<기안일><0001~9999>
  
![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/a7a72d7e-2ab8-4ee1-b1eb-dac98b9f084e)

- ### 결재 현황판

메인 페이지에 결재현황 생성

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/79fd0607-c06b-47f9-aae4-1c46fa471cd0)

</details>
<br>

### 24-02-07 업데이트
<details>
<summary> 자세히 보기 </summary>
  
- ### 전결처리 구현
  
결재선 지정 내, 전결 체크박스 체크 시 전결처리 구현

<br/>
  
![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/558af9e2-6a11-4502-8b6d-7435168f86f6)

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/1a0f9dd2-9204-4500-9caf-cfbf5bc1d425)

<br/>

- ### 상신취소 구현

최초의 승인 또는 반려가 발생하지 않은 결재건에 한해 상신취소 가능

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/e500dbc9-ce60-4ad1-ad76-50d49d2c0e5e)


- ### PowerAutomate 흐름 간소화 작업

기존에 흐름으로 구현한 조건을 Python 코드로 구현하여, 흐름 간소화 진행

### 1. [Flask전자결재] 기초 승인

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/0c06fff8-20fe-4532-bf18-8b6400722ca2)

<br/>

### 2. [Flask전자결재] 결재 알림

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/7bbf10ec-38e5-4d0f-a3e3-c93d7eeebd86)

<br/>

### 3. [Flask전자결재] 기초 결재 알림

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/d6887544-e94b-45e9-bb6f-41d382c30b2e)

<br/>

### 4. [Flask전자결재] 결재 완료 알림

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/750ad9aa-47cc-4650-89e0-9defee0c80f4)

<br/>

- ### Teams 메신저 알림 변경

Teams 메신저 내의 승인 기능을 사용하지 않고, 전자결재 앱의 문서 Detail 에서 승인 및 반려 처리 구현

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/5d650380-cdc1-42ad-a265-452a5df721cb)

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/6a0ad7cb-7373-430c-8666-89fa84ca7196)

<br/>

 - ### Navigate Bar 항목 수정

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/72fa605c-5490-4b1b-814f-b1fbfb2835b0)

</details>

<br>

### 24-02-08 업데이트
<details>
<summary> 자세히 보기 </summary>

- ### Login.html 아이디 저장 기능 구현

계정 기억하기 체크박스 체크시, localstorage에 계정명 저장

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/de78f45a-af21-4d98-9354-bf71a243ac56)

<br/>

- ### orgtree.html 결재선 저장 기능 구현

결재선 지정시, 결재선 저장 체크박스 체크시, localstorage에 결재자 정보, 전결 정보, 참조자 정보를 저장

<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/84a05227-9a48-4300-bb78-d34d982a8f80)

</details>

<br>

## **⭐️ PowerAutomate 로직**
<br>
<details>
<summary> 최초 로직설계 </summary>
  <br/>
  <details>
  <summary> 전체 로직 </summary>
  <br/>
    
  ![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/b63bee07-cf71-4c86-873a-4eb158fbf0cb)

  </details><br>

  <details>
  - <summary> 참조 로직 </summary>
  <br/>
    
  ![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/6e2ab02f-09c9-4b08-ad3a-2d66d0e97f5a)
  </details><br>

  <details>
  - <summary> 승인 로직 </summary>
  <br/>
    
  ![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/c42cf813-474d-4741-8d9d-a52a42dbcf4d)

  </details><br>
</details>

### 1. [Flask전자결재] 기초 승인
<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/0c06fff8-20fe-4532-bf18-8b6400722ca2)

### 2. [Flask전자결재] 결재 알림
<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/7bbf10ec-38e5-4d0f-a3e3-c93d7eeebd86)

### 3. [Flask전자결재] 기초 결재 알림
<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/d6887544-e94b-45e9-bb6f-41d382c30b2e)

### 4. [Flask전자결재] 결재 완료 알림
<br/>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/750ad9aa-47cc-4650-89e0-9defee0c80f4)

<br/>

## **💎 DB 정보**
<br>
<details>
<summary> 최초 DB설계 </summary>

![image](https://github.com/JunbeomCho22/RG_Approval/assets/156159216/cd168155-c040-46d9-9774-82db873b2967)
</details><br>

![image](https://github.com/JunbeomCho22/Radiantgrace_Approval/assets/156159216/5616b24e-c382-4fdc-b24c-ce1f84d33bb5)


<br />

## **🚀 배포**

- 배포는 Azure Web Service에 웹앱을 생성한 후 Local Git 으로 진행합니다[^1].

- ### 첫 배포
~~~terminal
git init
git add -A
git commit -m "커밋 내용"
git remote add <이름지정> <git-url>
git push <지정한이름> master
~~~

- ### 수정 후 배포
~~~terminal
git add -A
git commit -m "커밋 내용"
git push <지정한이름> master
~~~

<br />

## **🔗 참고자료**
[^1]: https://learn.microsoft.com/ko-kr/azure/app-service/deploy-local-git?tabs=cli
