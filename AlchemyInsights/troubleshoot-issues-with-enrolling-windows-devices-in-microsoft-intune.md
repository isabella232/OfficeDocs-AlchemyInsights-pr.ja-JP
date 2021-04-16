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
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="faecf-102">Microsoft Intune での Windows デバイスの登録に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="faecf-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="faecf-103">今すぐ問題を解決するには、以下のリソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="faecf-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="faecf-104">一般的なエラー メッセージと解決手順をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="faecf-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="faecf-p101">**このソフトウェアをインストールできません (0x80cf4017):** ご使用のアカウント証明書が期限切れです。Intune 管理コンソールで PC クライアント ソフトウェア パッケージを再ダウンロードします。詳しくは、このドキュメントを確認してください。</span><span class="sxs-lookup"><span data-stu-id="faecf-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span>
  
 <span data-ttu-id="faecf-108">**エラー コード 0x801c0003:** このエラーは次のシナリオで生じる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="faecf-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="faecf-p102">ユーザーがデバイスの制限を超える数のデバイスを登録しています。こちらのドキュメントを参照して、[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)してください。</span><span class="sxs-lookup"><span data-stu-id="faecf-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="faecf-111">[ユーザーはデバイスを Azure AD に参加させることができます] が、[なし] に設定されています。</span><span class="sxs-lookup"><span data-stu-id="faecf-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="faecf-112">すべてに設定するか、ユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="faecf-112">Set it to all or select users.</span></span> <span data-ttu-id="faecf-113">詳細については、[このドキュメント](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)でご確認ください。</span><span class="sxs-lookup"><span data-stu-id="faecf-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="faecf-p104">デバイスが他のユーザーによって既に登録済みです。その場合には、Azure Intune コンソールから対象デバイスを削除するか、デバイスを手動で登録解除してから、もう一度試します。</span><span class="sxs-lookup"><span data-stu-id="faecf-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="faecf-p105">Windows 10 Home デバイスです。Azure Active Directory に参加できるのは、Windows 10 Pro、Education SKU、Enterprise SKU のみです。</span><span class="sxs-lookup"><span data-stu-id="faecf-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="faecf-118">問題の解決に役立つその他のリソース:</span><span class="sxs-lookup"><span data-stu-id="faecf-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="faecf-p106">[Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="faecf-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="faecf-121">登録および解決を妨げる一般的なエラーの一覧については、[トラブルシューティングのガイド](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="faecf-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="faecf-122">[Microsoft Intune で Windows デバイスを登録する方法の詳細をご確認ください](https://docs.microsoft.com/intune/windows-enroll)。</span><span class="sxs-lookup"><span data-stu-id="faecf-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
