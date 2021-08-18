---
title: DKIM レコードの書式設定に関する一般的な問題を修正する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323995"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>DKIM レコードの書式設定に関する一般的な問題を修正する

ほとんどの DKIM セットアップの問題は、不適切な DNS レコードに関連しています。

DKIM セットアップの問題を修正するには、DKIM CNAME レコード (TXT レコード **ではありません**) の書式が正しいことを確認します。 詳細については、「[Office 365 で DKIM を手動でセットアップする手順](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)」を参照してください。

DNS レコード全般についてサポートが必要な場合は、「[任意の DNS ホスティング プロバイダーで Office 365 用に DNS レコードを作成する](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)」を参照してください。

**注**: ドメインの DNS ホスティング サービスで DKIM DNS レコードを作成または更新した後、DNS レコードが伝達されるのを待つ必要があります。
