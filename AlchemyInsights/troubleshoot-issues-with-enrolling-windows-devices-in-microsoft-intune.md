---
title: Microsoft Intune の Windows デバイスの登録に関する問題をトラブルシューティングします。
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661549"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Microsoft Intune の Windows デバイスの登録に関する問題をトラブルシューティングします。

これで問題を解決するのには下記のリソースを確認します。 
  
いくつかの一般的なエラー メッセージと解決方法の手順を使用して:
  
 **ソフトウェアをインストールすることはできません、0x80cf4017:** アカウント証明書の有効期限が切れています。Intune 管理コンソールで PC クライアント ソフトウェア パッケージを再度ダウンロードします。詳細についてはこのドキュメントを確認します。 
  
 **エラー コード 0x801c0003:** エラーは、次のシナリオで発生します。 
  
1. ユーザーは、デバイスの制限値よりも登録されているより多くのデバイスを持っています。[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限値を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)するのにはこれらのドキュメントを確認します。
    
2. 「ユーザー参加デバイス Azure AD に」は、「なし」に設定されています。すべて] に設定するか、選択のユーザーです。詳細については[このドキュメント](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)を確認します。 
    
3. デバイスは既に別のユーザーによって登録されています。Azure Intune コンソールからデバイスを削除する場合は、または、再試行する前に、デバイスを手動で unenroll。
    
4. デバイスは、Windows 10 ホームです。のみ Windows 10 Pro、教育およびエンタープライズ版 Sku は、Azure Active Directory に参加できます。
    
お客様の問題を解決するための他のリソース:
  
1. [Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。 
    
2. 各登録と解決策を防ぐための一般的なエラーの一覧については、これらのドキュメントを確認する:[トラブルシューティング ガイド](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)です。
    
[Microsoft Intune の Windows デバイスを登録する方法について説明](https://docs.microsoft.com/intune/windows-enroll)します。
  

