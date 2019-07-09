---
title: Microsoft Intune での Windows デバイスの登録に関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353542"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="bbf8b-102">Microsoft Intune での Windows デバイスの登録に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="bbf8b-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="bbf8b-103">今すぐ問題を解決するには、以下のリソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="bbf8b-104">一般的なエラー メッセージと解決手順をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="bbf8b-p101">**このソフトウェアをインストールできません (0x80cf4017):** ご使用のアカウント証明書が期限切れです。Intune 管理コンソールで PC クライアント ソフトウェア パッケージを再ダウンロードします。詳しくは、このドキュメントを確認してください。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span>
  
 <span data-ttu-id="bbf8b-108">**エラー コード 0x801c0003:** このエラーは次のシナリオで生じる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="bbf8b-p102">ユーザーがデバイスの制限を超える数のデバイスを登録しています。こちらのドキュメントを参照して、[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)してください。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="bbf8b-p103">[ユーザーはデバイスを Azure AD に参加させることができます] が [なし] に設定されています。[すべて] に設定するか、ユーザーを選択します。詳しくは、[こちらのドキュメント](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="bbf8b-p104">デバイスが他のユーザーによって既に登録済みです。その場合には、Azure Intune コンソールから対象デバイスを削除するか、デバイスを手動で登録解除してから、もう一度試します。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="bbf8b-p105">Windows 10 Home デバイスです。Azure Active Directory に参加できるのは、Windows 10 Pro、Education SKU、Enterprise SKU のみです。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="bbf8b-118">問題の解決に役立つその他のリソース:</span><span class="sxs-lookup"><span data-stu-id="bbf8b-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bbf8b-p106">[Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="bbf8b-121">登録および解決を妨げる一般的なエラーの一覧については、[トラブルシューティングのガイド](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="bbf8b-122">[Microsoft Intune で Windows デバイスを登録する方法の詳細をご確認ください](https://docs.microsoft.com/intune/windows-enroll)。</span><span class="sxs-lookup"><span data-stu-id="bbf8b-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
