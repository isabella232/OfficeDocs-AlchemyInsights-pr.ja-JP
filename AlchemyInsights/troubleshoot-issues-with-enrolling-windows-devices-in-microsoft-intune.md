---
title: Microsoft Intune での Windows デバイスの登録に関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808976"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Microsoft Intune での Windows デバイスの登録に関する問題のトラブルシューティング

今すぐ問題を解決するには、以下のリソースを確認します。
  
一般的なエラー メッセージと解決手順をいくつか示します。
  
 **このソフトウェアをインストールできません (0x80cf4017):** ご使用のアカウント証明書が期限切れです。Intune 管理コンソールで PC クライアント ソフトウェア パッケージを再ダウンロードします。詳しくは、このドキュメントを確認してください。
  
 **エラー コード 0x801c0003:** このエラーは次のシナリオで生じる可能性があります。
  
-  ユーザーがデバイスの制限を超える数のデバイスを登録しています。こちらのドキュメントを参照して、[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)してください。

-  [ユーザーはデバイスを Azure AD に参加させることができます] が、[なし] に設定されています。 すべてに設定するか、ユーザーを選択します。 詳細については、[このドキュメント](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)でご確認ください。

-  デバイスが他のユーザーによって既に登録済みです。その場合には、Azure Intune コンソールから対象デバイスを削除するか、デバイスを手動で登録解除してから、もう一度試します。

-  Windows 10 Home デバイスです。Azure Active Directory に参加できるのは、Windows 10 Pro、Education SKU、Enterprise SKU のみです。

問題の解決に役立つその他のリソース:
  
-  [Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。

-  登録および解決を妨げる一般的なエラーの一覧については、[トラブルシューティングのガイド](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)をご覧ください。

[Microsoft Intune で Windows デバイスを登録する方法の詳細をご確認ください](https://docs.microsoft.com/intune/windows-enroll)。
