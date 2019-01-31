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
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="1a9b0-102">Microsoft Intune で Android のデバイスの登録に関する問題をトラブルシューティングします。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="1a9b0-103">これで問題を解決するのには下記のリソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="1a9b0-104">いくつかの一般的な問題と解決手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="1a9b0-p101">**デバイスが暗号化されていない会社のポータルでのエラー:** V7.0 では、特にからのアプリの新しいバージョンでは、デバイスが完全に暗号化されているかどうかを確認するのには起動時のパスコードが必要です。共通のソリューションは、スタートアップの暗証番号 (pin) を有効にするか、デバイスを完全に暗号化すること。詳細については[このドキュメント](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)を確認します。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="1a9b0-p102">**Intune サービスにチェック_インまたは Intune 管理コンソールで「問題」として表示するデバイスが失敗する:** いくつかの Samsung 4.4 と 5.5 のデバイスは、サービスにチェックがあります。この問題に 3 つの可能な解決策があります。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="1a9b0-110">Intune 会社のポータル アプリケーションでは、デバイスの同期を自動的に開始を手動で開きます。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="1a9b0-111">Android 6.0 またはそれ以上のデバイスを更新します。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="1a9b0-p103">Intune 企業ポータルの管理から、Samsung スマート マネージャーを無効にします。これらの問題と解決策の詳細については[このドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)を確認します。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="1a9b0-p104">**ユーザー ライセンスの種類が無効**または**エラーのユーザー名は認識されません:** Intune または EMS のライセンスを割り当てられる必要があるユーザーです。を通じてライセンスを割り当てるにはこれらのドキュメントを確認します。 Office 管理者センターまたは Azure ポータルです。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="1a9b0-116">お客様の問題を解決するための他のリソース:</span><span class="sxs-lookup"><span data-stu-id="1a9b0-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1a9b0-p105">[Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="1a9b0-119">登録できない一般的なエラーと各エラーの解決策の一覧については、[このドキュメント](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="1a9b0-120">[Microsoft Intune で Android のデバイスを登録する方法について説明](https://docs.microsoft.com/intune/android-enroll)します。</span><span class="sxs-lookup"><span data-stu-id="1a9b0-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

