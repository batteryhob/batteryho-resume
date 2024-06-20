---
description: 카트라이더 전적 검색 서비스 | https://tmi.nexon.com/kart
---

# Nexon TMI

{% hint style="info" %}
_vue vuex react redux sass ejs chartjs webpack .net framework django aws-elasticbeanstalk_ 이(가) 사용되었습니다.
{% endhint %}

![카트라이더 전적 검색 서비스](../../../.gitbook/assets/tmi.gif)

![모바일 화면](../../../.gitbook/assets/mobile.gif)

## Overview <a href="#overview" id="overview"></a>

{% embed url="https://tmi.nexon.com/kart" %}

롤의 op.gg와 비슷한 성격의 카트라이더 유저들을 위한 전적 검색 사이트입니다. 큰 호응을 받은 서비스라 좋은 평가 후, 차기작을 위한 후속 프로젝트 준비 중입니다.

{% embed url="https://www.youtube.com/watch?v=_YBOOiU-1OU" %}

{% embed url="https://www.youtube.com/watch?v=V1qFVpWCnpw" %}

## How did you resolve major issue?

#### 트랙로그를 활용할 수 없을까?

넥슨에서는 카트라이더의 모든 주행로그를 관리합니다. 이를 이용하여  사용자에게 재미있는 콘텐츠를 제공할 수 없을까 고민하다가 주행로그의 외곽선 데이터를 추출할 수 있다는 사실을 알게 된 후, 직접 구현한 콘텐츠 입니다.&#x20;

트랙로그는 굉장히 많은 데이터라 일반 DB에서는 퍼포먼스가 떨어지므로 Nosql 테이블을 구현해 스트링 형태로 데이터 분석가에게 저장을 요청했습니다. FrontApp에서는 이를 파싱하여 D3를 이용한 비주얼 라이징을 구현해냈습니다.&#x20;

{% content-ref url="d3.md" %}
[d3.md](d3.md)
{% endcontent-ref %}

