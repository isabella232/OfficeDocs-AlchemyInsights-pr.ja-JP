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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="6300d-102">Microsoft Intune で iOS デバイスの登録に関する問題をトラブルシューティングします。</span><span class="sxs-lookup"><span data-stu-id="6300d-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="6300d-103">これで問題を解決するのには下記のリソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="6300d-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="6300d-104">いくつかの一般的なエラー メッセージと解決方法の手順を使用して:</span><span class="sxs-lookup"><span data-stu-id="6300d-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="6300d-p101">**デバイスの上限に達しました**ユーザーは、デバイスの制限値よりも登録されているより多くのデバイスを持っています。[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限値を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)するのにはこれらのドキュメントを確認します。</span><span class="sxs-lookup"><span data-stu-id="6300d-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="6300d-p102">**このサービスはサポートされていません。登録ポリシーが:** Apple プッシュ通知サービス (APN) を構成するか、更新する必要があります。実行する方法の詳細については、[このドキュメント](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)を確認します。</span><span class="sxs-lookup"><span data-stu-id="6300d-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="6300d-p103">**無効なユーザー ライセンスの種類またはユーザー名を認識できません:** ユーザーは、Intune または EMS のライセンスを割り当てる必要があります。を通じてライセンスを割り当てるにはこれらのドキュメントを確認します。 [Office 管理者センター](https://docs.microsoft.com/intune/licenses-assign)または[Azure ポータル](https://docs.microsoft.com/azure/active-directory/license-users-groups)です。</span><span class="sxs-lookup"><span data-stu-id="6300d-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="6300d-111">お客様の問題を解決するための他のリソース:</span><span class="sxs-lookup"><span data-stu-id="6300d-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6300d-p104">[Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6300d-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="6300d-114">各登録と解決策を防ぐための一般的なエラーの一覧については、これらのドキュメントを確認する:[トラブルシューティング ガイド](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)です。</span><span class="sxs-lookup"><span data-stu-id="6300d-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="6300d-115">[Microsoft Intune で iOS デバイスを登録する方法について説明](https://docs.microsoft.com/intune/ios-enroll)します。</span><span class="sxs-lookup"><span data-stu-id="6300d-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

