# **🎬 MoviePick** 
## 하이브리드 필터링 × LLM 기반 정교화된 영화 추천
> **P-Semester Project**  
> _Precision & Personalization, powered by Hybrid Recommender Systems and Large Language Models_

---

## 📌 프로젝트 배경
기존 VOD/OTT 추천 엔진은  
- **행동 데이터**(시청 이력, 별점 등)와 **콘텐츠 메타데이터**(장르, 감독, 배우 등)에 주로 의존합니다.  
- 기본적인 개인화는 가능하지만, **심층적 선호 파악**·**동적 취향 변화 반영**에는 한계가 있습니다.  

---

## 🧠 핵심 아이디어
1. **하이브리드 필터링**  
   - _Collaborative_ + _Content-Based_ 접근을 통합해 cold-start 위험을 완화하고 기본 선호도를 파악합니다.  
2. **LLM 추가 계층**  
   - **Meta-Llama / Llama-3.2-1B** 로 **리뷰·검색 로그·자연어 코멘트**를 임베딩 →  
     - 영화 간 **의미 기반 유사도**를 벡터 수준에서 정밀 추정  
     - 사용자의 **세부 취향·감정 톤**까지 모델링  
3. **다단계 랭킹 파이프라인**  
   1) 기본 Hybrid Score  
   2) LLM Vector Similarity 보정  

---

## 📱 애플리케이션 흐름

### 1) 초기 설문조사로 취향 입력 & 로그인 후 화면

<div align="center">
  <img src="https://github.com/user-attachments/assets/fc4ae9ed-293a-4045-8584-749ff9b5e016">
</div>


### 2) 영화 추천 화면 & 추천 이유 설명 

<div align="center">
  <img src="https://github.com/user-attachments/assets/4ad0cb40-6cbc-48b2-9a90-700789580a42">
</div>

---


## 🏗️ 시스템 아키텍처

![5](https://github.com/user-attachments/assets/342b2f5f-ad51-4a2f-ae10-6e05441a8914)

## DB 설계 
<img width="1744" height="1392" alt="ERD_MODEL" src="https://github.com/user-attachments/assets/a9d4f87d-9ba0-461d-8f96-66078c88450a" />

## AI 시스템 아키텍쳐 
<img width="569" height="427" alt="image" src="https://github.com/user-attachments/assets/253b0ab3-de8c-44fa-ab93-00afb8d3bad2" />


---

## 🎬 시연 영상

https://github.com/user-attachments/assets/4fd1c407-5b0f-4bba-b3a8-ddf03fd384e0


## 👤 Team Members

| Avatar | 이름&nbsp;/&nbsp;영문 | 담당 영역 | 핵심 기술스택 | GitHub |
|:---:|:---|:---|:---|:---:|
| <img src="https://github.com/Jae-Hyuk-Jang.png" width="100"/> | **장재혁**<br/>Jae-Hyuk Jang | AI 백엔드 엔지니어<br/>AI 서버–백엔드 연동 및 서버 통합 관리<br/>DB 설계 | FastAPI&nbsp;&#124; Spring Boot&nbsp;&#124; Python&nbsp; | [Jae-Hyuk-Jang](https://github.com/Jae-Hyuk-Jang) |
| <img src="https://github.com/axhtl.png" width="100"/> | **유수빈**<br/>Su-Bin Yoo | 백엔드 개발<br/>DB 설계 및 팀 일정 관리 | Spring Boot&nbsp;&#124; JPA&nbsp;&#124; MySQL | [axhtl](https://github.com/axhtl) |
| <img src="https://github.com/SongInseo01.png" width="100"/> | **송인서**<br/>In-Seo Song | AI 엔지니어<br/>영화 데이터 수집 및 AI 모델 구축 | PyTorch&nbsp;&#124; Pandas&nbsp;&#124; Scikit-Learn | [SongInseo01](https://github.com/SongInseo01) |
| <img src="https://github.com/taejuIRIS.png" width="100"/> | **김태주**<br/>Tae-Joo Kim | 프론트엔드 개발<br/>UI/UX 설계 및 구현 | React&nbsp;&#124; Figma&nbsp;&#124; Tailwind CSS | [taejuIRIS](https://github.com/taejuIRIS) |
