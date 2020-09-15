---
title: Microsoft Intune での Android デバイスの登録に関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689959"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="90e63-102">Microsoft Intune での Android デバイスの登録に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="90e63-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="90e63-103">今すぐ問題を解決するには、以下に一覧表示されているリソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="90e63-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="90e63-104">一般的な問題と解決手順をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="90e63-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="90e63-p101">**ポータル サイトでデバイスが暗号化されないエラー:** Android の新しいバージョン (詳しくは v7.0 以降) では、デバイスが完全に暗号化されているかどうかを確認するためにスタートアップ パスコードが必要です。一般的な解決策は、スタートアップ PIN を有効にするか、デバイスを完全に暗号化することです。詳細については、[このドキュメント](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="90e63-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="90e63-p102">**デバイスが Intune サービスでのチェックインに失敗する、または Intune 管理コンソールに "異常" として表示される:** Samsung 4.4 と 5.5 の一部のデバイスで、サービスにチェックインできない場合があります。この問題に対しては、考えられる解決策が 3 つあります。</span><span class="sxs-lookup"><span data-stu-id="90e63-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="90e63-110">Intune ポータル サイト アプリを手動で開きます。これによりデバイスの同期が自動的に開始されます。</span><span class="sxs-lookup"><span data-stu-id="90e63-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="90e63-111">デバイスを Android 6.0 以降に更新します。</span><span class="sxs-lookup"><span data-stu-id="90e63-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="90e63-p103">Intune ポータル サイトの管理から Samsung Smart Manage を無効にします。これらの問題と解決方法の詳細については、[こちらのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="90e63-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="90e63-p104">**ユーザー ライセンスの種類が無効**または**ユーザー名が認識されないエラー:** ユーザーには、Intune または EMS ライセンスが割り当てられている必要があります。Office 管理センターまたは Azure portal からライセンスを割り当てるには、こちらのドキュメントを確認してください。</span><span class="sxs-lookup"><span data-stu-id="90e63-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="90e63-116">問題の解決に役立つその他のリソース:</span><span class="sxs-lookup"><span data-stu-id="90e63-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="90e63-p105">[Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90e63-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="90e63-119">登録できない一般的なエラーと各エラーの解決策の一覧については、[このドキュメント](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90e63-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="90e63-120">[Microsoft Intune で Android デバイスを登録する方法を学習します](https://docs.microsoft.com/intune/android-enroll)。</span><span class="sxs-lookup"><span data-stu-id="90e63-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
