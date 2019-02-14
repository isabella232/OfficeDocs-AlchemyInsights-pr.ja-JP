---
title: Microsoft Intune での Windows デバイスの登録に関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934781"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Microsoft Intune での Windows デバイスの登録に関する問題のトラブルシューティング

今すぐ問題を解決するには、以下のリソースを確認します。 
  
一般的なエラー メッセージと解決手順をいくつか示します。
  
 **このソフトウェアをインストールできません (0x80cf4017):** ご使用のアカウント証明書が期限切れです。Intune 管理コンソールで PC クライアント ソフトウェア パッケージを再ダウンロードします。詳しくは、このドキュメントを確認してください。 
  
 **エラー コード 0x801c0003:** このエラーは次のシナリオで生じる可能性があります。 
  
1. ユーザーがデバイスの制限を超える数のデバイスを登録しています。こちらのドキュメントを参照して、[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)してください。
    
2. [ユーザーはデバイスを Azure AD に参加させることができます] が [なし] に設定されています。[すべて] に設定するか、ユーザーを選択します。詳しくは、[こちらのドキュメント](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)をご覧ください。 
    
3. デバイスが他のユーザーによって既に登録済みです。その場合には、Azure Intune コンソールから対象デバイスを削除するか、デバイスを手動で登録解除してから、もう一度試します。
    
4. Windows 10 Home デバイスです。Azure Active Directory に参加できるのは、Windows 10 Pro、Education SKU、Enterprise SKU のみです。
    
問題の解決に役立つその他のリソース:
  
1. [Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。 
    
2. 登録および解決を妨げる一般的なエラーの一覧については、[トラブルシューティングのガイド](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)をご覧ください。
    
[Microsoft Intune で Windows デバイスを登録する方法の詳細をご確認ください](https://docs.microsoft.com/intune/windows-enroll)。
  

