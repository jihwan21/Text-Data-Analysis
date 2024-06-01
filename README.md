# Text-Data-Analysis

---
## 1. 배경 & 목적
주관 : 전공수업 텍스트데이터분석  
목적 : Web Crawling으로 수집한 Text Data를 전처리하고 모델링하여 수집한 분야를 잘 분류하는지 분석

---
## 2. 담당 역할
- Individual
- 데이터 수집
- 데이터 전처리
- 모델링 및 결과 분석
---
## 3. 프로젝트 진행 과정
### 1. 텍스트 데이터 수집
- 검색 Keywords 7개
  1. Object Detection
  2. Natural Language Processing
  3. Time Series Analysis
  4. Speech Recognition
  5. Semantic Segmentation
  6. Image Generation
  7. Sentiment Analysis

- 데이터 수집 Source
  1. Naver blog
  2. Naver news
  3. arXiv

- 데이터 수집 방법  
  1. Selenium 활용 arXiv  
  2. Naver 검색 API 활용 Naver blog & news

### 2. 텍스트 데이터 전처리
- 전처리에 필요한 함수 정의(URL, 특수기호&문자 제거, 띄어쓰기 교정 등)
- 한글, 영어 텍스트 데이터 분리하여 각각 전처리 진행

### 3. 모델링
1. **Wordcloud** : keyword 7 개 (English&Korean text data = blog + news + arXiv)  
각 키워드 별로 어떤 단어가 비중을 많이 차지하고 있는지 해석  
영어와 한글로 나누어 모델링 하였음  
2. **LDA** : keyword 7 개 하나로 합쳐서 진행 English text data blog + news + arXiv)  
LDA결과로 나온 토픽 7 개 분석해 keyword 랑 잘 매칭되는지 확인 모델링 결과 topic 과 keyword 특정해보기  
토픽 모델링이 잘 수행되었는지 해석  
3. **LSTM 을 이용한 다중 분류 모델** : keyword 7 개 데이터 하나로 합쳐서 진행 (English text data)  
LSTM 기반 분류 모델이 텍스트 데이터가 주어졌을 때 7 개의 키워드로 잘 분류하는지 확인  
(데이터를 아래와 같이 두 가지 경우로 나누어 진행)  
3-1. arXiv 텍스트 데이터만 주어졌을 때  
3 2. arXiv 데이터에 + news & blog 텍스트 데이터도 함께 주어졌을 때   

## 4. 성과
- 텍스트 데이터 수집 및 전처리 경험
- 3가지 모델링(Worldcloud / LDA / LSTM을 이용한 다중 분류 모델) 진행 및 분석

## 5. 자료
[최종 발표.pdf](https://drive.google.com/file/d/1O4O7Gd_2KFH4CtcozfdP16cNyAWhtokE/view?usp=drive_link)
