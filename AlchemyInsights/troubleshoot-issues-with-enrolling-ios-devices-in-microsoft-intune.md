---
title: Microsoft Intune での iOS デバイスの登録に関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047981"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Microsoft Intune での iOS デバイスの登録に関する問題のトラブルシューティング

今すぐ問題を解決するには、以下のリソースを確認します。 
  
一般的なエラー メッセージと解決手順をいくつか示します。
  
- **デバイスの上限に達しました** ユーザーがデバイスの制限を超える数のデバイスを登録しています。こちらのドキュメントを参照して、[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)してください。
    
- **このサービスはサポートされていません。登録ポリシーがありません:** Apple Push Notification Service (APN) を構成するか、更新する必要があります。方法については、[こちらのドキュメント](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)をご確認ください。 
    
- **ユーザー ライセンスの種類が無効またはユーザー名が認識されません:** ユーザーには、Intune または EMS ライセンスが割り当てられている必要があります。[Office 管理センター](https://docs.microsoft.com/intune/licenses-assign)または [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups) からライセンスを割り当てるには、こちらのドキュメントを確認してください。
    
問題の解決に役立つその他のリソース:
  
1. [Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。 
    
2. 登録および解決を妨げる一般的なエラーの一覧については、[トラブルシューティングのガイド](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)をご覧ください。
    
3. [Microsoft Intune で iOS デバイスを登録する方法の詳細をご確認ください](https://docs.microsoft.com/intune/ios-enroll)。
    

