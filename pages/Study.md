---
layout: page
title: "Study Notes"
permalink: /study/
---

# Study Notes

AI/ML을 공부하며 정리한 저장소들입니다. 세부 내용보다는 중요한 순서대로 핵심만 요약했습니다.

## [CV_Study](https://github.com/gaeun-k/CV_Study)
성신여대·성균관대·덕성여대 학생 5명이 함께하는 10주 컴퓨터비전 스터디 (2~5주차 Cassava, 6~10주차 Wheat Detection).
- **Cassava Leaf Disease Classification**: EDA, baseline 모델, augmentation, 하이퍼파라미터 튜닝
- **Global Wheat Detection**: YOLO 기반 객체 탐지, bounding box · IoU · mAP

## [CIFAR10_Pytorch](https://github.com/gaeun-k/CIFAR10_Pytorch)
CIFAR-10 이미지 분류 CNN을 단계적으로 개선해 본 실습 프로젝트.
- Baseline CNN → BatchNorm, SGD+momentum, LR scheduling 적용 (정확도 79.75% → 84.49%)
- CIFAR-10 입력 크기에 맞춘 ResNet18 직접 구현 (3x3 conv, stride 조정 등)

## [kaggle-study](https://github.com/gaeun-k/kaggle-study)
5명이 함께한 8주 Kaggle 컴퓨터비전 스터디 (Cassava Leaf Disease Classification, Global Wheat Detection).
- 대회별 EDA · baseline · 실험 내용을 주차별로 기록

## [TIL](https://github.com/gaeun-k/TIL)
딥러닝, 알고리즘, 인턴십 경험을 꾸준히 기록한 학습 저장소.
- 딥러닝 기초(회귀, 경사하강법, 퍼셉트론/역전파), 알고리즘(BFS/DFS, 이진탐색 등), Kaggle 실습(LightGBM/XGBoost, CNN, LSTM)

## [Class_ML](https://github.com/gaeun-k/Class_ML)
머신러닝 수업 실습 코드 모음.
- 베이지안 분류기, 퍼셉트론(XOR), 당뇨 예측 신경망, 범주형 데이터 전처리 등

---

## Blog Posts

{% for post in site.posts %}
  {% if post.categories contains "study" %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%Y-%m-%d" }}
  {% endif %}
{% endfor %}
