---
description: 서든어택 실시간 월핵탐지 서비스 | 넥슨 인텔리전스 랩스 사내 서비스
---

# Nexon WallhackDetector

{% hint style="info" %}
_vue vuex sass ejs webpack gulp node graphql-yoga docker kubernetes aws-eks_ 이(가) 사용되었습니다.
{% endhint %}

![키보드와 마우스 동작하는 서든어택 월핵탐지 시스템](../../../.gitbook/assets/sawh3.gif)

## Overview&#x20;

머신러닝 학습을 위한 자동화 도구를 편하게 제공하기 위해 기획과 디자인 및 설계하여 구현했습니다. 클릭만으도 머신러닝을 위한 작업이 진행되며, 쿠버네테스를 알지 못해도 쿠버네티스 환경에서 모델 학습, 검증, 배포가 가능하도록 만들었습니다.

## How did you resolve major issue?

#### 1. 좀 더 손쉽게 단순 업무를 수행할 수 있을까?

단순 작업을 하는 사용자를 위해 키보드로만 처리할 수 있도록 키보드 동작을 핸들링 했습니다.

#### 2. 하루 8만 건의 데이터를 실시간으로 처리할 수 있을까?

쿠버네티스 환경을 웹서비스 노드와 데이터처리 노드로 분리하고  Cronjob을 사용해 실시간으로 처리했습니다. GPU를 사용한 리소스를 충분히 쓰면서도 웹 서비스를 안정적으로 운영할 수 있었고, 하나의 클러스터에서 관리에 관리 프로세스를 간단히 할 수 있었습니다.&#x20;

#### 3. 민감한 핵 제제관련 자료들을 API의 추가 개발없이 손쉽게 제공할 수 있을까?

Node기반의 GraphQL 서버로 백엔드를 구성하여 같은 API로 필요한 정보만 조회할 수 있도록 만들었습니다.&#x20;

{% content-ref url="graphql.md" %}
[graphql.md](graphql.md)
{% endcontent-ref %}

