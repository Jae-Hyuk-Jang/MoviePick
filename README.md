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

### 1) 초기 설문조사로 취향 입력  
사용자는 첫 로그인 시 선호 장르, 분위기, 선호 감독 등의 정보를 선택해 취향을 입력합니다.

![초기 설문조사](https://github.com/user-attachments/assets/582c3193-4683-415c-b3a5-11c75d5e95fa)

---

### 2) 로그인 후 메인 화면  
맞춤형 대시보드를 통해 최신 추천 영화, 인기 콘텐츠, 사용자 맞춤 큐레이션을 제공합니다.

![로그인 후 화면](https://github.com/user-attachments/assets/847e6e24-66b6-4608-a160-e18deae4cd4d)

---

### 3) 영화 추천 화면  
하이브리드 + LLM 분석을 바탕으로 현재 시점에서 가장 적합한 영화를 추천합니다.

![영화 추천 화면](https://github.com/user-attachments/assets/1ec48b7a-1c4c-406b-910a-929d725850d0)

---

### 4) 영화 추천 이유 설명  
추천 이유는 LLM이 분석한 자연어 리뷰, 장르 유사도, 감정 톤 분석 등을 바탕으로 제시됩니다.  
이를 통해 사용자는 단순 추천이 아닌 **납득 가능한 추천 이유**를 확인할 수 있습니다.

![추천 이유 설명 1](https://github.com/user-attachments/assets/b6da5c2e-20a3-4d33-9858-26e889aa6f19)  
![추천 이유 설명 2](https://github.com/user-attachments/assets/70fb02d6-189f-4411-a601-5e09fed47c23)


---


## 🏗️ 시스템 아키텍처

![architechture](https://github.com/user-attachments/assets/709a242f-d582-4174-8358-1e63ca67058d)

---

## 🎬 시연 영상

https://github.com/user-attachments/assets/4fd1c407-5b0f-4bba-b3a8-ddf03fd384e0

