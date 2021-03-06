---

copyright:
  years: 2014, 2017
lastupdated: "2017-10-03"

keywords:

subcollection: image-templates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 이미지 템플리트 정보
{: #about-image-templates}

표준 이미지 템플리트는 운영 체제와는 무관하게 모든 {{site.data.keyword.BluVirtServers_short}}에 대한 이미징 옵션을 제공합니다.
{:shortdesc}

표준 이미지 템플리트를 사용하면 기존 가상 서버의 이미지가 캡처되고, 캡처된 이미지를 기반으로 새 이미지를 작성할 수 있습니다. 표준 이미지 템플리트는 베어메탈 서버와 호환 가능하지 않습니다.

## 이미지 템플리트 작동 방법
이미지 템플리트에 대한 두 개의 기본 조치는 작성 및 배치입니다. 이미지 작성을 요청하는 경우, {{site.data.keyword.BluSoftlayer_full}}의 자동화된 시스템은 사용자의 서버를 오프라인 상태로 전환합니다. 서버가 오프라인 상태인 동안에는 데이터의 압축된 백업이 작성되고, 구성 정보가 기록되며 이미지 템플리트가 {{site.data.keyword.BluSoftlayer_notm}} SAN에 저장됩니다. 이미지 템플리트의 배치 단계 중에 자동화된 시스템은 선택된 이미지에서 수집된 데이터를 기반으로 하는 새 서버를 생성합니다. 배치 프로세스는 볼륨을 조정하고 복사된 데이터를 복원한 후에 새 호스트에 대한 최종 구성 변경사항(예: 네트워크 구성)을 작성합니다.

## 개인용 이미지

개인용 이미지는 해당 계정에서 사용자가 작성한 이미지 또는 다른 계정에서 작성되어 공유되는 이미지입니다. 기본적으로 작성된 모든 이미지는 개인용입니다.

## 공용 이미지

공용 이미지는 {{site.data.keyword.BluSoftlayer_notm}}에서 게시하거나 고객이 공용화했으며, 모든 {{site.data.keyword.BluSoftlayer_notm}} 고객이 사용할 수 있는 사전 구성된 가상 서버입니다. 공용 이미지 템플리트를 통해 프로비저닝된 가상 서버는 일반적으로 서로 다른 구성 스펙의 특정 조합을 사용하여 최적의 성능을 유지하도록 구성되어 있습니다.
