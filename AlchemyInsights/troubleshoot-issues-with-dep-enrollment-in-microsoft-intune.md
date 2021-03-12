---
title: Microsoft Intune での DEP 登録に関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: f76e47c2a3007175ae1bfbd9d20cb59513eb713b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708715"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Microsoft Intune での DEP 登録に関する問題のトラブルシューティング

今すぐ問題を解決するには、以下のリソースを確認します。
  
1. DEP デバイスを登録できず、MFA (Multi-Factor Authentication) が有効な場合には、MFA を無効にしてください。現在、DEP 登録では MFA はサポートされていません。

2. [Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。

3. 登録および解決を妨げる一般的なエラーの一覧については、[トラブルシューティングのガイド](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)をご覧ください。

4. [デバイス登録プログラムについてご確認ください](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)。
