---
title: Microsoft Intune で iOS デバイスの登録に関する問題をトラブルシューティングします。
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477395"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Microsoft Intune で iOS デバイスの登録に関する問題をトラブルシューティングします。

これで問題を解決するのには下記のリソースを確認します。 
  
いくつかの一般的なエラー メッセージと解決方法の手順を使用して:
  
- **デバイスの上限に達しました**ユーザーは、デバイスの制限値よりも登録されているより多くのデバイスを持っています。[デバイスを削除](https://docs.microsoft.com/en-us/intune/devices-wipe)するか、[デバイスの制限値を変更](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)するのにはこれらのドキュメントを確認します。
    
- **このサービスはサポートされていません。登録ポリシーが:** Apple プッシュ通知サービス (APN) を構成するか、更新する必要があります。実行する方法の詳細については、[このドキュメント](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get)を確認します。 
    
- **無効なユーザー ライセンスの種類またはユーザー名を認識できません:** ユーザーは、Intune または EMS のライセンスを割り当てる必要があります。を通じてライセンスを割り当てるにはこれらのドキュメントを確認します。 [Office 管理者センター](https://docs.microsoft.com/en-us/intune/licenses-assign)または[Azure ポータル](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups)です。
    
お客様の問題を解決するための他のリソース:
  
1. [Intune トラブルシューティングのポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を使用して、診断し、一般的な登録の失敗を解決します。詳細については[このドキュメント](https://docs.microsoft.com/en-us/intune/help-desk-operators)を確認します。 
    
2. 各登録と解決策を防ぐための一般的なエラーの一覧については、これらのドキュメントを確認する:[トラブルシューティング ガイド](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)です。
    
3. [Microsoft Intune で iOS デバイスを登録する方法について説明](https://docs.microsoft.com/en-us/intune/ios-enroll)します。
    

