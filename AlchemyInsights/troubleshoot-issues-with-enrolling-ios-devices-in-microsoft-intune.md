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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28298293"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="46cc1-102">Microsoft Intune で iOS デバイスの登録に関する問題をトラブルシューティングします。</span><span class="sxs-lookup"><span data-stu-id="46cc1-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="46cc1-103">これで問題を解決するのには下記のリソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="46cc1-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="46cc1-104">いくつかの一般的なエラー メッセージと解決方法の手順を使用して:</span><span class="sxs-lookup"><span data-stu-id="46cc1-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="46cc1-p101">**デバイスの上限に達しました**ユーザーは、デバイスの制限値よりも登録されているより多くのデバイスを持っています。[デバイスを削除](https://docs.microsoft.com/en-us/intune/devices-wipe)するか、[デバイスの制限値を変更](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)するのにはこれらのドキュメントを確認します。</span><span class="sxs-lookup"><span data-stu-id="46cc1-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="46cc1-p102">**このサービスはサポートされていません。登録ポリシーが:** Apple プッシュ通知サービス (APN) を構成するか、更新する必要があります。実行する方法の詳細については、[このドキュメント](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get)を確認します。</span><span class="sxs-lookup"><span data-stu-id="46cc1-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="46cc1-p103">**無効なユーザー ライセンスの種類またはユーザー名を認識できません:** ユーザーは、Intune または EMS のライセンスを割り当てる必要があります。を通じてライセンスを割り当てるにはこれらのドキュメントを確認します。 [Office 管理者センター](https://docs.microsoft.com/en-us/intune/licenses-assign)または[Azure ポータル](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups)です。</span><span class="sxs-lookup"><span data-stu-id="46cc1-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="46cc1-111">お客様の問題を解決するための他のリソース:</span><span class="sxs-lookup"><span data-stu-id="46cc1-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="46cc1-p104">[Intune トラブルシューティングのポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を使用して、診断し、一般的な登録の失敗を解決します。詳細については[このドキュメント](https://docs.microsoft.com/en-us/intune/help-desk-operators)を確認します。</span><span class="sxs-lookup"><span data-stu-id="46cc1-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="46cc1-114">各登録と解決策を防ぐための一般的なエラーの一覧については、これらのドキュメントを確認する:[トラブルシューティング ガイド](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)です。</span><span class="sxs-lookup"><span data-stu-id="46cc1-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="46cc1-115">[Microsoft Intune で iOS デバイスを登録する方法について説明](https://docs.microsoft.com/en-us/intune/ios-enroll)します。</span><span class="sxs-lookup"><span data-stu-id="46cc1-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

