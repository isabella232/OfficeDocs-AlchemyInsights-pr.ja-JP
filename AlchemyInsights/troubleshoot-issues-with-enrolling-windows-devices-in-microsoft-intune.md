---
title: Microsoft Intune の Windows デバイスの登録に関する問題をトラブルシューティングします。
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661549"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="5d72e-102">Microsoft Intune の Windows デバイスの登録に関する問題をトラブルシューティングします。</span><span class="sxs-lookup"><span data-stu-id="5d72e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="5d72e-103">これで問題を解決するのには下記のリソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="5d72e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="5d72e-104">いくつかの一般的なエラー メッセージと解決方法の手順を使用して:</span><span class="sxs-lookup"><span data-stu-id="5d72e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="5d72e-p101">**ソフトウェアをインストールすることはできません、0x80cf4017:** アカウント証明書の有効期限が切れています。Intune 管理コンソールで PC クライアント ソフトウェア パッケージを再度ダウンロードします。詳細についてはこのドキュメントを確認します。</span><span class="sxs-lookup"><span data-stu-id="5d72e-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="5d72e-108">**エラー コード 0x801c0003:** エラーは、次のシナリオで発生します。</span><span class="sxs-lookup"><span data-stu-id="5d72e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="5d72e-p102">ユーザーは、デバイスの制限値よりも登録されているより多くのデバイスを持っています。[デバイスを削除](https://docs.microsoft.com/intune/devices-wipe)するか、[デバイスの制限値を変更](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)するのにはこれらのドキュメントを確認します。</span><span class="sxs-lookup"><span data-stu-id="5d72e-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="5d72e-p103">「ユーザー参加デバイス Azure AD に」は、「なし」に設定されています。すべて] に設定するか、選択のユーザーです。詳細については[このドキュメント](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)を確認します。</span><span class="sxs-lookup"><span data-stu-id="5d72e-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="5d72e-p104">デバイスは既に別のユーザーによって登録されています。Azure Intune コンソールからデバイスを削除する場合は、または、再試行する前に、デバイスを手動で unenroll。</span><span class="sxs-lookup"><span data-stu-id="5d72e-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="5d72e-p105">デバイスは、Windows 10 ホームです。のみ Windows 10 Pro、教育およびエンタープライズ版 Sku は、Azure Active Directory に参加できます。</span><span class="sxs-lookup"><span data-stu-id="5d72e-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="5d72e-118">お客様の問題を解決するための他のリソース:</span><span class="sxs-lookup"><span data-stu-id="5d72e-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="5d72e-p106">[Intune トラブルシューティング ポータル](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)を利用して、診断し、一般的な登録エラーを解決します。詳細については、[このドキュメント](https://docs.microsoft.com/intune/help-desk-operators)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d72e-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="5d72e-121">各登録と解決策を防ぐための一般的なエラーの一覧については、これらのドキュメントを確認する:[トラブルシューティング ガイド](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)と[トラブルシューティングのドキュメント](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)です。</span><span class="sxs-lookup"><span data-stu-id="5d72e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="5d72e-122">[Microsoft Intune の Windows デバイスを登録する方法について説明](https://docs.microsoft.com/intune/windows-enroll)します。</span><span class="sxs-lookup"><span data-stu-id="5d72e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

