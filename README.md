## **개요**

- **프로젝트명**: 합성 데이터의 성능 평가를 위한 통계적 데이터 분석
- **목적**: 실제 데이터와의 분포 비교를 통해 합성 데이터의 품질을 평가하여, 다양한 인공지능 모델 학습 데이터로서의 활용성을 검토하고 개선 방안을 제시
- **주제 선정 배경**: 합성 데이터의 수요가 증가함에 따라, 데이터 품질을 평가하는 지표의 필요성이 증대됨. 이를 통해 합성 데이터의 정확한 품질 평가를 제공하고, 향후 AI 학습의 신뢰도를 높일 수 있음

## 사용기술

---

- **합성 데이터 생성**: DCGAN을 사용하여 실제 데이터와 유사한 합성 데이터를 생성
- **차원 축소 및 시각화**: t-SNE를 사용하여 고차원 이미지를 2차원으로 축소해 분포 시각화
- **분포 비교 및 유사도 검증**: 커널 밀도 추정 및 K-Means 클러스터링을 통해 두 데이터의 유사도를 비교, 스미르노프 검정으로 통계적 유사도 확인
- **통계 분석 도구**: Python의 Seaborn 및 Scipy 패키지를 사용하여 분석 시각화 및 통계 검증

## **역할 및 주요 기여**

- **아이디어 기획**: 증가하는 합성 데이터의 품질 문제를 해결하기 위한 통계적 데이터 분석 프로젝트 구상
- **데이터 분석 및 모델링**:
- DCGAN을 활용한 합성 데이터 생성 및 실제 데이터와의 분포 비교를 위한 전처리 및 분석 수행
- t-SNE를 통한 차원 축소, K-Means 클러스터링으로 레이블링 작업, 커널 밀도 추정을 통해 실제 데이터와의 분포 유사도 시각화
- 비모수 검정(스미르노프 검정)을 통해 합성 데이터와 실제 데이터의 통계적 분포 차이를 분석하여 품질을 객관적으로 평가

## **성과 및 배운 점**

- **성과**: 합성 데이터의 품질 평가에 있어 통계적 접근 방식을 도입함으로써, 단순한 시각적 유사도 평가를 넘어 실질적인 데이터 품질 지표를 도출. 이는 향후 다양한 인공지능 모델의 학습 데이터로 활용 시 유용한 기준이 될 수 있음
- **배운 점**:
    - 데이터 품질 평가를 위해 비모수 검정을 포함한 다양한 통계 기법을 활용하는 방법을 학습하며, 기존의 통계 이론과 AI 데이터 분석이 융합될 수 있음을 이해
    - DCGAN과 같은 생성 모델의 데이터 품질을 객관적으로 평가하기 위해 차원 축소, 클러스터링, 밀도 추정 등 다양한 분석 방법을 적용하는 경험을 통해 분석 방법론의 다양성을 체득

## 결과

- **주요 결과**: 합성 데이터가 실제 데이터와 분포의 유사성을 갖추었으나, 일부 경계에서는 불명확함을 보여, 합성 데이터의 개선 여지를 확인
- **통계적 유의미성 확인**: 스미르노프 검정을 통해 합성 데이터와 실제 데이터의 분포가 유사하지 않음을 확인, 추가적인 품질 평가와 개선 방향 필요성 제안

## 보완할 점

- **추가 검증 방법 도입**: PCA, LDA와 같은 다른 차원 축소 기법을 활용하여 데이터 분포 평가를 다각화하고, 추가적인 비모수 검정 기법 도입 필요
- **딥러닝 모델 적용**: 향후 중요 변수를 추출해 합성 데이터의 품질을 더 명확히 평가하기 위해 다양한 딥러닝 모델로 확장

## 원페이퍼 보고서
![2023 경영경제대학 학술제 원페이퍼 보고서_인공지능탐정단](https://github.com/user-attachments/assets/b6c2fc45-d893-4869-9425-54c12328c210)

