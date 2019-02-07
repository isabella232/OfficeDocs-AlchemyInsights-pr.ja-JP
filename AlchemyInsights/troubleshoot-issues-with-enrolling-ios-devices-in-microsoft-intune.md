---
title: Microsoft Intune での iOS デバイスの登録に関する問題のトラブルシューティング
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658444"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="40083-102">Microsoft Intune での iOS デバイスの登録に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="40083-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="40083-103">今すぐ問題を解決するには、以下のリソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="40083-103">Review resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="40083-104">一般的なエラー メッセージと解決手順をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="40083-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="40083-p101">**デバイスの上限に達しました** ユーザーがデバイスの制限を超える数のデバイスを登録しています。こちらのドキュメントを参照して、[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)してください。</span><span class="sxs-lookup"><span data-stu-id="40083-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="40083-p102">**このサービスはサポートされていません。登録ポリシーがありません:** Apple Push Notification Service (APN) を構成するか、更新する必要があります。方法については、[こちらのドキュメント](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="40083-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="40083-p103">**ユーザー ライセンスの種類が無効またはユーザー名が認識されません:** ユーザーには、Intune または EMS ライセンスが割り当てられている必要があります。[Office 管理センター](https://docs.microsoft.com/intune/licenses-assign)または [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups) からライセンスを割り当てるには、こちらのドキュメントを確認してください。</span><span class="sxs-lookup"><span data-stu-id="40083-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="40083-111">問題の解決に役立つその他のリソース:</span><span class="sxs-lookup"><span data-stu-id="40083-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="40083-p104">[Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40083-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="40083-114">登録および解決を妨げる一般的なエラーの一覧については、[トラブルシューティングのガイド](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="40083-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="40083-115">[Microsoft Intune で iOS デバイスを登録する方法の詳細をご確認ください](https://docs.microsoft.com/intune/ios-enroll)。</span><span class="sxs-lookup"><span data-stu-id="40083-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

