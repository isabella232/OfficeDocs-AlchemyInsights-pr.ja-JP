---
title: Microsoft Intune での Android デバイスの登録に関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500076"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsoft Intune での Android デバイスの登録に関する問題のトラブルシューティング

今すぐ問題を解決するには、以下に一覧表示されているリソースを確認します。
  
一般的な問題と解決手順をいくつか示します。
  
 **ポータル サイトでデバイスが暗号化されないエラー:** Android の新しいバージョン (詳しくは v7.0 以降) では、デバイスが完全に暗号化されているかどうかを確認するためにスタートアップ パスコードが必要です。一般的な解決策は、スタートアップ PIN を有効にするか、デバイスを完全に暗号化することです。詳細については、[このドキュメント](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)をご確認ください。
  
 **デバイスが Intune サービスでのチェックインに失敗する、または Intune 管理コンソールに "異常" として表示される:** Samsung 4.4 と 5.5 の一部のデバイスで、サービスにチェックインできない場合があります。この問題に対しては、考えられる解決策が 3 つあります。
  
1. Intune ポータル サイト アプリを手動で開きます。これによりデバイスの同期が自動的に開始されます。

2. デバイスを Android 6.0 以降に更新します。

3. Intune ポータル サイトの管理から Samsung Smart Manage を無効にします。これらの問題と解決方法の詳細については、[こちらのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)を確認してください。

 **ユーザー ライセンスの種類が無効**または**ユーザー名が認識されないエラー:** ユーザーには、Intune または EMS ライセンスが割り当てられている必要があります。Office 管理センターまたは Azure portal からライセンスを割り当てるには、こちらのドキュメントを確認してください。
  
問題の解決に役立つその他のリソース:
  
1. [Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。

2. 登録できない一般的なエラーと各エラーの解決策の一覧については、[このドキュメント](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)を参照してください。

3. [Microsoft Intune で Android デバイスを登録する方法を学習します](https://docs.microsoft.com/intune/android-enroll)。
