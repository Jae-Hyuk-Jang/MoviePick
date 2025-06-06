# MoviePick – 하이브리드 필터링 × LLM 기반 정교화된 영화 추천
> **P-Semester Project**  
> _Precision & Personalization, powered by Hybrid Recommender Systems and Large Language Models_

## 1. 프로젝트 배경
기존 VOD/OTT 추천 엔진은  
- **행동 데이터**(시청 이력, 별점 등)와 **콘텐츠 메타데이터**(장르, 감독, 배우 등)에 주로 의존합니다.  
- 기본적인 개인화는 가능하지만, **심층적 선호 파악**·**동적 취향 변화 반영**에는 한계가 있습니다.  

## 2. 핵심 아이디어
1. **하이브리드 필터링**  
   - _Collaborative_ + _Content-Based_ 접근을 통합해 cold-start 위험을 완화하고 기본 선호도를 파악합니다.  
2. **LLM 추가 계층**  
   - **Meta-Llama / Llama-3.2-1B** 로 **리뷰·검색 로그·자연어 코멘트**를 임베딩 →  
     - 영화 간 **의미 기반 유사도**를 벡터 수준에서 정밀 추정  
     - 사용자의 **세부 취향·감정 톤**까지 모델링  
3. **다단계 랭킹 파이프라인**  
   1) 기본 Hybrid Score  
   2) LLM Vector Similarity 보정  
   3) 실시간 컨텍스트(시간, 기기, 시청 상태) Re-Rank  

## 🏗️ 시스템 아키텍처

![architechture](https://github.com/user-attachments/assets/709a242f-d582-4174-8358-1e63ca67058d)


## 🎬 시연 영상

https://github.com/user-attachments/assets/4fd1c407-5b0f-4bba-b3a8-ddf03fd384e0

