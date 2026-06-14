# Feature Engineering 파이프라인 구현 및 성능 비교 실험

**학번/이름:** 2353683 / 김남규  
**데이터셋:** Titanic Dataset (생존 여부 예측 - Classification)  
**제출일:** 2026-06-14

---

## 과제 개요

Titanic 데이터셋을 활용하여 결측치 처리 · 인코딩 · 스케일링 · 파생 변수 생성 등  
Feature Engineering 파이프라인을 설계하고, 전처리 전략에 따른 모델 성능 차이를 비교·분석한다.

## 실험 구성

| 실험 | 결측치 처리 | 인코딩 | 스케일링 | Feature Selection |
|------|-------------|--------|----------|-------------------|
| Base | 행 제거 | Label | 없음 | X |
| Exp-1 | Mean | One-Hot | Standard | X |
| Exp-2 | Median | Label | MinMax | SelectKBest |
| Exp-3 | Most Frequent | One-Hot | Robust | RFE |

## 사용 모델

- Logistic Regression
- Random Forest
- XGBoost
- LightGBM

## 가산점 항목

- sklearn Pipeline 객체 활용
- GridSearchCV 하이퍼파라미터 최적화
- SHAP 기반 설명 가능성 분석
- Feature Importance 다중 모델 시각화 고도화

## 파일 구성

| 파일 | 설명 |
|------|------|
| `(과제) 특성공학 파이프라인 김남규.ipynb` | 전체 분석 코드 |
