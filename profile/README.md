# AI 활용 소아과의사 진단 보조 서비스 SoAI

AI를 활용하여 소아과의사의 업무를 효율적으로 할 수 있게 도와주는 서비스를 기획 및 구현했습니다.
> 1. DICOM 파일 포맷 이미지뷰어와 이미지 편집 툴을 제공
> 2. CNN 모델을 통해 의료이미지를 분석해서 질환 부위를 표시(Segmentation)
> 3. 의료이미지와 이전 질환 내역을 동시에 분석해서 예측되는 질환을 설명(X-Diag)
> 4. 전문 의료 지식을 통해 파인튜닝한 LLM을 통해 질의에 대한 답변을 받을 수 있는 챗봇 기능

위 기능을 제공하고 있습니다.

# :vhs:️ 프로토타입 영상
[![SoAI 유튜브 시연 영상](https://img.youtube.com/vi/J77fvXnbVy8/0.jpg)](https://www.youtube.com/watch?v=J77fvXnbVy8)

:exclamation:️ 위 썸네일을 누르시면 시연영상을 볼 수 있습니다.

# :briefcase: 프로젝트 구성
| Repo | Description | Tech |
|------|-------------|------|
| [frontend](https://github.com/soai-org/soai-frontend) | 사용자 UI 및 이미지 뷰어 구현 | ![Next JS](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white) ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) ![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white) |
| [backend](https://github.com/soai-org/soai-springboot) | REST API & 인증 권한 관리 & 데이터 관리 | ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white) ![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white) |
| [ai-server](https://github.com/soai-org/soai-fastapi) | AI 모델 및 추론 기능 서빙 서버 | ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi) ![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)|

# :people_hugging: 팀 소개
- 강두훈(프로젝트 총괄)
  - 일정 및 산출물 관리
  - UI/UX 개발
  - Cornerstone.js DICOM 포맷 파일 이미지 렌더링
 

- 황유성(프로젝트 리더)
  - 프로젝트 아디이어 기획
  - 복부 x-ray 의료사진 분석 및 예측 모델 개발
  - AI 기능 서빙 API 구현
 
- 김도연
  - DB 스키마 정의 및 SQL문 작성
  - 인증 권한 기능 구현
  - 피부 질환 진단 AI 모델 구현
 

- 임수열
  - 초음파 사진 분석 충수염 예측 모델 개발
 

- 전유범
  - Orthanc REST API 요청 로직 구현
  - Thumbnail 요청 최적화


# :gear: 시스템 구성
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1dc449cc-92ce-404c-8946-75ed5f92741b" />

# 화면 자료
[로그인 화면: 서비스 이용 초기 인증 요청을 위한 화면]
<img width="1892" height="1024" alt="스크린샷 2025-09-03 오후 3 03 15" src="https://github.com/user-attachments/assets/a4540ba1-7e79-4dd1-83f8-8eea125f727b" />

[메인 화면: 환자와 스터디 리스트 조회 화면]
<img width="1891" height="1024" alt="스크린샷 2025-09-03 오후 3 05 03" src="https://github.com/user-attachments/assets/8309db40-35ed-43dc-9baf-1e7256092eb0" />

[이미지 뷰어 화면 - 1: 의료이미지 상호작용 뷰어]
<img width="1894" height="1025" alt="스크린샷 2025-09-03 오후 3 05 33" src="https://github.com/user-attachments/assets/280520c3-2c3f-4316-a06b-2428acab9a43" />

[이미지 뷰어 화면 - 2: AI 사용 후]
<img width="1891" height="1026" alt="스크린샷 2025-09-04 오전 11 17 00" src="https://github.com/user-attachments/assets/5f3e623a-59eb-4316-b2e4-e7b4613248c0" />

[사용자 관리 화면: 사용자 조회 및 추가/수정/삭제 기능 요청 화면]
<img width="1894" height="1025" alt="스크린샷 2025-09-03 오후 3 05 57" src="https://github.com/user-attachments/assets/5308b93c-acdc-41e2-89b9-01a9f6e556d2" />


# 참고자료
### [프로젝트 보고서](https://drive.google.com/file/d/1sWhmiKX7Afz_UrdEt1nxj92HauiCjlmi/view?usp=drive_link)
> 프로젝트 설계 및 구현 과정 등을 자세히 살펴볼 수 있는 산출물입니다.
