---
layout: page
title: Projects
permalink: /projects/
---

## AI-Travel-Recommendation
감정 기반 여행지 추천 시스템. 다국어 CLIP을 파인튜닝해 사용자의 감정과 여행지 이미지 사이의 의미적 관계를 학습했습니다.

- **Tech**: CLIP(ViT-B/32) 파인튜닝, Multilingual DistilBERT, FAISS 벡터 검색, Supervised Contrastive Learning
- **Features**: 장면 분류(13종) + 감정 정렬 듀얼 헤드 구조, 텍스트↔이미지 / 이미지↔이미지 검색
- **Repo**: <https://github.com/gaeun-k/AI-Travel-Recommendation>

{% for post in site.posts %}
  {% if post.categories contains "ai-travel-recommendation" %}
- **포스팅**: [{{ post.title }}]({{ post.url }})
  {% endif %}
{% endfor %}

---

## AAC-Scene-Recognition-AI
스마트 글래스(Meta Glass)로 촬영한 이미지를 분석해 현재 상황(장면)을 인식하고, 알맞은 AAC(보완대체의사소통) 카드를 추천하는 시스템입니다.

- **Tech**: OpenCLIP 기반 장면 분류, FastAPI 백엔드
- **Features**: 병원 접수처·약국·카페·식당·편의점 계산대, 버스/지하철 입구 등 7종 장면 분류, Swagger API 문서
- **Repo**: <https://github.com/gaeun-k/AAC-Scene-Recognition-AI>

{% for post in site.posts %}
  {% if post.categories contains "aac-scene-recognition-ai" %}
- **포스팅**: [{{ post.title }}]({{ post.url }})
  {% endif %}
{% endfor %}

---

## Face2Voice
텍스트와 얼굴 이미지를 입력하면 **얼굴 정체성을 반영한 음성**을 합성하는 Flask 데모입니다.

- **Tech**: PyTorch, Flask, facenet_pytorch, SV2TTS 스타일 파이프라인, ShuffleNetV2 (Lip2Speech 기반)
- **Repo**: <https://github.com/gaeun-k/Face2Voice>
- **포스팅**: [/face2voice/](/face2voice/)

---

## Moms-touch *(바이브코딩 프로젝트)*
말이나 글로만 전해지던 엄마·할머니의 손맛 레시피를 AI로 구조화해 기록하고 공유하는 모바일 앱입니다.

- **Tech**: React Native(Expo) + TypeScript, FastAPI, PostgreSQL, GPT-4o-mini, Google STT/TTS
- **Features**: 음성→레시피 변환, 지역 기반 레시피 지도, 맞춤 추천(지역·난이도), 단계별 음성 안내, 좋아요/프로필
- **Repo**: <https://github.com/gaeun-k/Moms-touch>

{% for post in site.posts %}
  {% if post.categories contains "moms-touch" %}
- **포스팅**: [{{ post.title }}]({{ post.url }})
  {% endif %}
{% endfor %}
