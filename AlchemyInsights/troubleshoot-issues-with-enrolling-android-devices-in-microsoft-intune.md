---
title: Microsoft Intune で Android のデバイスの登録に関する問題をトラブルシューティングします。
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655888"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsoft Intune で Android のデバイスの登録に関する問題をトラブルシューティングします。

これで問題を解決するのには下記のリソースを確認します。
  
いくつかの一般的な問題と解決手順を実行します。
  
 **デバイスが暗号化されていない会社のポータルでのエラー:** V7.0 では、特にからのアプリの新しいバージョンでは、デバイスが完全に暗号化されているかどうかを確認するのには起動時のパスコードが必要です。共通のソリューションは、スタートアップの暗証番号 (pin) を有効にするか、デバイスを完全に暗号化すること。詳細については[このドキュメント](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)を確認します。 
  
 **Intune サービスにチェック_インまたは Intune 管理コンソールで「問題」として表示するデバイスが失敗する:** いくつかの Samsung 4.4 と 5.5 のデバイスは、サービスにチェックがあります。この問題に 3 つの可能な解決策があります。 
  
1. Intune 会社のポータル アプリケーションでは、デバイスの同期を自動的に開始を手動で開きます。
    
2. Android 6.0 またはそれ以上のデバイスを更新します。
    
3. Intune 企業ポータルの管理から、Samsung スマート マネージャーを無効にします。これらの問題と解決策の詳細については[このドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)を確認します。 
    
 **ユーザー ライセンスの種類が無効**または**エラーのユーザー名は認識されません:** Intune または EMS のライセンスを割り当てられる必要があるユーザーです。を通じてライセンスを割り当てるにはこれらのドキュメントを確認します。 Office 管理者センターまたは Azure ポータルです。 
  
お客様の問題を解決するための他のリソース:
  
1. [Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。 
    
2. 登録できない一般的なエラーと各エラーの解決策の一覧については、[このドキュメント](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)を参照してください。 
    
3. [Microsoft Intune で Android のデバイスを登録する方法について説明](https://docs.microsoft.com/intune/android-enroll)します。
    

