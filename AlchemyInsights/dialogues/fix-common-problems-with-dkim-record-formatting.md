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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527827"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>DKIM レコードの書式設定に関する一般的な問題を修正する

ほとんどの DKIM セットアップの問題は、不適切な DNS レコードに関連しています。

DKIM セットアップの問題を修正するには、DKIM CNAME レコード (TXT レコード **ではありません**) の書式が正しいことを確認します。 詳細については、「[Office 365 で DKIM を手動でセットアップする手順](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)」を参照してください。

DNS レコード全般についてサポートが必要な場合は、「[任意の DNS ホスティング プロバイダーで Office 365 用に DNS レコードを作成する](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)」を参照してください。

> [!NOTE]
> ドメインの DNS ホスティン グサービスで DKIM DNS レコードを作成または更新したら、その DNS レコードが伝達されるまで待機する必要があります。
