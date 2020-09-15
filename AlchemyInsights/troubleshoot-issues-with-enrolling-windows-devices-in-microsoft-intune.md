---
title: Microsoft Intune での Windows デバイスの登録に関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658883"
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

-  登録および解決を妨げる一般的なエラーの一覧については、[トラブルシューティングのガイド](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)をご覧ください。

[Microsoft Intune で Windows デバイスを登録する方法の詳細をご確認ください](https://docs.microsoft.com/intune/windows-enroll)。
