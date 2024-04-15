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
<br>![1](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/aacd0904-33e3-4163-848b-d8cac406c50a)


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
  <details>
  <summary> 최초 로그인 페이지 구성 </summary>

  <br>

  ![2](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/1262d73f-0dc1-4e6b-b5de-04c84f7b49e7)<br/>

  - 기존에 사용하던 Microsoft 365 계정과 동일한 계정으로 로그인
  <br>

  </details><br>

![print](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/67e60233-1b62-4274-84e4-51d97dde2540)

- Microsoft 365 계정을 사용하여 로그인

<br/>

### 2. 문서결재 요청 구현
<br>

![3](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/3edb91ac-9eb2-4fec-b493-20fdafee23a0)<br/>


- 가장 기본적인 기안 양식을 HTML로 구현
<br/>

  ### 2-1. DatePicker 사용으로 날짜선택<br>
  <details>
  <summary> DatePicker </summary>

  ![4](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/e80c38d4-161b-454d-bace-f3c797220b08)<br/>


  - Bootstrap 기능인 DatePicker 사용
  </details><br>

  ### 2-2. 결재선 지정 기능<br>
  <details>
  <summary> 결재선 </summary>
    
  ![5](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/691e139f-9ca4-4948-a454-2d633c913241)<br/>


  - <결재선 지정> 버튼 클릭 시 새창으로 결재선 지정 창 구현
  - 결재선 지정 시, 각각 결재자, 참조자 이름 문서에 자동 기입 구현
  - 결재선 지정 시, '제출'버튼 visible 구현
  </details><br/>

  ### 2-3. 파일 업로드<br>
  <details>
  <summary> 파일 업로드 </summary>

  ![6](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/9a32ab09-5c2c-4ce9-96c5-78cc4197f671)<br/>


  - 로컬 파일을 업로드하여 첨부파일 기능 구현
  - 여러개의 파일 동시에 업로드 기능 구현
  </details><br>

### 3. 메신저 알림 구현 (MS Teams)
<details>
<summary> 기존 알림 구현 </summary>

<br>
  
![7](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/29c2a444-aaa8-4f56-8c05-f7599200115d)![8](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/cd7de8f3-ca8d-4ec4-8840-87f0975bdbde)
<br/>

- 사내 메신저 (MS Teams)로 결재진행 및 참조 알림 기능 구현

</details>

<br>

![9](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/2c2250b9-0c6a-4989-bad1-54e26e43bc97)

<br>

![10](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/ddd1d471-f1a1-42c8-b9fc-7cbd17d60cee)

- 흐름봇을 통한 결재사항 및 URL 알림 구현
- 전자결재 앱의 문서 Detail 에서 승인 및 반려 처리 구현



<br>

### 4. 결재 문서 열람
<br>

![11](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/f1649b6d-7daa-4c0c-8619-33019b8acdbb)<br/>

- 기안자 열 값이 현재 로그인 중인 유저의 계정 값과 일치하는 문서들만 출력
<br>

### 4-1. 문서 상세보기<br>
<details>
<summary> 문서 상세보기 </summary>

![12](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/3e02a7b0-f602-48ae-be76-6941818697e4)<br/>


- 작성된 문서 열람 및 결재 진행 상황 확인 가능
</details><br>

### 4-2. 프린트<br>
<details>
<summary> 프린트 </summary>

![13](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/d6016e53-8ff9-4efa-88d4-7b88fcbc3bc1)<br/>


- 프린트 버튼으로 필요한 양식만 출력 기능 구현
</details><br>

### 4-3. 첨부파일<br>
<details>
<summary> 첨부파일 </summary>

![14](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/dab8b071-b8ec-4cf6-a717-875a8494f419)<br/>


- 문서 하단 업로드된 첨부파일 열기 || 저장 기능 구현
</details><br>

## **💾 업데이트**

### 24-01-25 업데이트
<details>
<summary> 자세히 보기 </summary>
  
- ### 문서번호 자동생성 및 적용
  
예) CJH-<기안일><0001~9999>

![15](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/5ef7f951-9be0-46af-9ca0-248b1268a49c)


- ### 결재 현황판

메인 페이지에 결재현황 생성

![16](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/ad3cbf65-a1f2-4a84-8e81-b14dd17b012f)


</details>
<br>

### 24-02-07 업데이트
<details>
<summary> 자세히 보기 </summary>
  
- ### 전결처리 구현
  
결재선 지정 내, 전결 체크박스 체크 시 전결처리 구현

<br/>

![17](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/a90359fc-5488-4b51-a4df-dfe91f20f97f)

<br/>

![18](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/521740d6-0fcc-4f42-a45d-d0d66ac294a3)

<br/>

- ### 상신취소 구현

최초의 승인 또는 반려가 발생하지 않은 결재건에 한해 상신취소 가능

<br/>

![19](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/2db17af2-170b-4936-aa97-37b5a64b165f)



- ### PowerAutomate 흐름 간소화 작업

기존에 흐름으로 구현한 조건을 Python 코드로 구현하여, 흐름 간소화 진행

### 1. [Flask전자결재] 기초 승인

<br/>

![20](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/30639bde-156b-4386-927e-bed836a02a80)


<br/>

### 2. [Flask전자결재] 결재 알림

<br/>

![21](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/ddc37407-b5fd-4972-8d32-8cd4a405bbc2)


<br/>

### 3. [Flask전자결재] 기초 결재 알림

<br/>

![22](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/31d9398b-92fa-4794-9343-5753707d973d)


<br/>

### 4. [Flask전자결재] 결재 완료 알림

<br/>

![23](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/6b8dd381-1f8a-4415-9677-83296c00150c)


<br/>

- ### Teams 메신저 알림 변경

Teams 메신저 내의 승인 기능을 사용하지 않고, 전자결재 앱의 문서 Detail 에서 승인 및 반려 처리 구현

<br/>

![24](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/1c882f37-1dd7-4643-81e9-f4935fc847ee)


<br/>

![25](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/c1f45e09-4d51-4856-b1e1-e11b090ec67e)


<br/>

 - ### Navigate Bar 항목 수정

<br/>

![26](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/9a4e98d0-2ddb-454d-a3b3-4a4972eeeea7)


</details>

<br>

### 24-02-08 업데이트
<details>
<summary> 자세히 보기 </summary>

- ### Login.html 아이디 저장 기능 구현

계정 기억하기 체크박스 체크시, localstorage에 계정명 저장

<br/>

![27](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/50e0bfd8-f8ae-486e-966b-efdb5827e45f)


<br/>

- ### orgtree.html 결재선 저장 기능 구현

결재선 지정시, 결재선 저장 체크박스 체크시, localstorage에 결재자 정보, 전결 정보, 참조자 정보를 저장

<br/>

![28](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/2c6d8eb4-1bfc-4368-8608-8ce0e36026db)


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
  
  ![29](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/5afd763c-ab8c-4d88-9067-63b3ba70bfbf)

  </details><br>

  <details>
  - <summary> 참조 로직 </summary>
  <br/>
    
  ![30](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/e61247ee-e5a7-456e-b5a0-d04c56398b0d)
  
  </details><br>

  <details>
  - <summary> 승인 로직 </summary>
  <br/>
    
  ![31](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/ef19251c-2c7b-45f7-8981-3636ff25371d)

  </details><br>
</details>

### 1. [Flask전자결재] 기초 승인
<br/>

![32](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/316e4b5d-55f9-46a1-89ad-aa698f35401d)


### 2. [Flask전자결재] 결재 알림
<br/>

![33](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/e86d6709-e8e1-446e-bd19-2891b3a7e8e5)


### 3. [Flask전자결재] 기초 결재 알림
<br/>

![34](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/7984bded-3456-403d-97c5-70ba4643ee77)


### 4. [Flask전자결재] 결재 완료 알림
<br/>

![35](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/a54e040e-e971-418c-9fb0-32dd15ebf6d8)

<br/>

## **💎 DB 정보**
<br>
<details>
<summary> 최초 DB설계 </summary>

![36](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/db04bb82-af3f-4ae1-a394-a7f1f36d550d)

</details><br>

![37](https://github.com/JunbeomCho22/portfolio-ApprovalSys/assets/156159216/134af058-5554-4b28-9c01-8472cb350ce6)



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
