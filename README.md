# Phishing Safe AI (Team 깜자와 꽁주)

Phishing Safe AI는 사용자가 입력한 메시지를 AI가 분석하여  
스팸인지 정상 메시지(햄)인지 즉시 판단하고,  
0~100 사이의 위험도 점수까지 제공하는 웹 기반 스팸·피싱 분석 서비스입니다.  
또한 OX 학습 기능을 통해 사용자가 직접 메시지를 판단해보며  
보안 인식을 자연스럽게 향상시킬 수 있도록 설계된 교육형 보안 서비스입니다.

## 주요 기능
- 메시지 입력 후 AI가 스팸/햄 분석 결과 즉시 제공  
- 스팸 가능성을 수치로 표현한 위험도 점수(0~100) 출력  
- 메시지 내부의 위험 요소(긴급성 문구, 금전 요구, 링크 등) 간단 설명  
- OX 방식의 스팸 학습 기능 제공  

## 기술 스택
- Python, Flask (웹 서버)
- Scikit-learn (SVM 모델, TF-IDF 벡터화)
- HTML / CSS (templates, static)
- Pickle (모델 및 벡터라이저 저장)

## 프로젝트 구조
app.py  
templates/  
static/  
final_model.pkl  
final_model_with_vectorizer.pkl  
final_200_sample_spam_ham_dataset.csv  

## 실행 방법
1. 필요한 패키지 설치  
   pip install flask scikit-learn

2. Flask 서버 실행  
   python app.py

3. 웹 브라우저 접속  
   http://127.0.0.1:5000/

## 데이터 출처
- 팀 자체 수집 한국어 이메일 스팸·햄 데이터  
- GitHub 공개 한국어 스미싱/문자 스팸 데이터셋

## 팀명
깜자와 꽁주
