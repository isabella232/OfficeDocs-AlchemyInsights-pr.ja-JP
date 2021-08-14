---
title: アプリケーション保護ポリシー
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: ab6ad9c4bf95ee013c66384ec8449ceb1b56e8f3ea9e95c695dbbab0e9fa3fc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969976"
---
# <a name="application-protection-policy"></a>アプリケーション保護ポリシー

アプリケーション保護ポリシー (APP) を初めて使用する場合は、[「アプリ保護ポリシーの概要」](https://docs.microsoft.com/intune/apps/app-protection-policy) を確認してください。

APP の使用を開始するには、[「アプリ保護ポリシーを作成して割り当てる方法」](https://docs.microsoft.com/intune/app-protection-policies) を参照してください。

アプリケーション保護ポリシーの要件:

- ユーザーが Intune または EMS ライセンスを持っています。
- ユーザーは、アプリケーション保護ポリシーの対象グループに属します。
- 1 人の企業ユーザーのみが、デバイス上の保護されたアプリにサインインします。
- アプリケーションは [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started) を実装しています。SDK をサポートするアプリのリストについては、「[Microsoft Intune 保護アプリ](https://docs.microsoft.com/intune/apps-supported-intune-apps)」を参照してください。

ポリシーは、上記の要件を満たしているユーザーが Intune SDK を有効にしたアプリにサインインすると適用されます。 ポリシーが適用されているかどうかを判断する最も簡単な方法は、ユーザーがポリシーにピンを設定することを要求することです。 

詳細については、以下を参照してください:

[APP/MAM のトラブルシューティングに関する FAQ](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[アプリ保護ポリシーのセットアップを検証する方法](https://docs.microsoft.com/intune/app-protection-policies-validate)

[アプリ保護ポリシーの配布タイミングを理解する](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[アプリ保護ポリシーを監視する方法](https://docs.microsoft.com/intune/app-protection-policies-monitor)