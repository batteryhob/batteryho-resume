---
description: 머신러닝 프로세스 자동화 서비스 | 넥슨 인텔리전스랩스 사내 서비스
---

# Nexon Nxflow

{% hint style="info" %}
_react redux sass ejs webpack gulp python flask docker kubernetes aws-ek&#x73;_&#xAC00; 사용되었습니다.
{% endhint %}

![Nxflow 동작 화면](../../../.gitbook/assets/nxflow.gif)

## Overview&#x20;

머신러닝 학습을 위한 자동화 도구를 편하게 제공하기 위해 기획과 디자인 및 설계하여 구현했습니다. 클릭만으도 머신러닝을 위한 작업이 진행되며, 쿠버네테스를 알지 못해도 쿠버네티스 환경에서 모델 학습, 검증, 배포가 가능하도록 만들었습니다.

## How did you resolve major issue?

#### 사용자로 하여금 쿠버네티스 지식없이 쿠버네티스를 쓰게할 수 있을까?

AWS의 eks cli를 설치한 버전의 컨테이너를 제작하여 해당 컨테이너 위에서 웹서비스를 구현했습니다. flask로 만든 해당 웹서비스는 환경 자체가 aws cli를 포함하고 있기 때문에 Rest api로 받은 파라미터들을 쿠버네티스 명령어로 파싱해 클릭만으로도 쿠버네티스의 동작이 가능하게 만들었습니다.&#x20;

{% content-ref url="kubernetes.md" %}
[kubernetes.md](kubernetes.md)
{% endcontent-ref %}

