---
title: Microsoft Intune での DEP 登録に関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 11b0d73c34996fd84431b38d77b64536d386977e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766714"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="5bd95-102">Microsoft Intune での DEP 登録に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="5bd95-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="5bd95-103">今すぐ問題を解決するには、以下のリソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="5bd95-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="5bd95-p101">DEP デバイスを登録できず、MFA (Multi-Factor Authentication) が有効な場合には、MFA を無効にしてください。現在、DEP 登録では MFA はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bd95-p101">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA. Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="5bd95-p102">[Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bd95-p102">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="5bd95-108">登録および解決を妨げる一般的なエラーの一覧については、[トラブルシューティングのガイド](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5bd95-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="5bd95-109">[デバイス登録プログラムについてご確認ください](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)。</span><span class="sxs-lookup"><span data-stu-id="5bd95-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
