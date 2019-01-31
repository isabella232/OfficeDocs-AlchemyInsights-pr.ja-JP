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
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658444"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Microsoft Intune で iOS デバイスの登録に関する問題をトラブルシューティングします。

これで問題を解決するのには下記のリソースを確認します。 
  
いくつかの一般的なエラー メッセージと解決方法の手順を使用して:
  
- **デバイスの上限に達しました**ユーザーは、デバイスの制限値よりも登録されているより多くのデバイスを持っています。[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限値を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)するのにはこれらのドキュメントを確認します。
    
- **このサービスはサポートされていません。登録ポリシーが:** Apple プッシュ通知サービス (APN) を構成するか、更新する必要があります。実行する方法の詳細については、[このドキュメント](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)を確認します。 
    
- **無効なユーザー ライセンスの種類またはユーザー名を認識できません:** ユーザーは、Intune または EMS のライセンスを割り当てる必要があります。を通じてライセンスを割り当てるにはこれらのドキュメントを確認します。 [Office 管理者センター](https://docs.microsoft.com/intune/licenses-assign)または[Azure ポータル](https://docs.microsoft.com/azure/active-directory/license-users-groups)です。
    
お客様の問題を解決するための他のリソース:
  
1. [Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。 
    
2. 各登録と解決策を防ぐための一般的なエラーの一覧については、これらのドキュメントを確認する:[トラブルシューティング ガイド](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)です。
    
3. [Microsoft Intune で iOS デバイスを登録する方法について説明](https://docs.microsoft.com/intune/ios-enroll)します。
    

