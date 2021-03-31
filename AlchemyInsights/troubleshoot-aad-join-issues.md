---
title: ハイブリッド Azure AD 参加のトラブルシューティング
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405859"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="78edd-102">ハイブリッド Azure AD 参加のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="78edd-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="78edd-103">初めてデバイス登録を設定する場合は、「[Azure Active Directory でのデバイス管理の概要](https://docs.microsoft.com/azure/active-directory/devices/overview)」を確認してください。このガイドでは、デバイスを Azure AD の制御下に配置する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="78edd-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="78edd-104">デバイスを Azure AD に直接登録し、それらを Intune に登録する場合は、[構成済み Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) があり、最初に[ライセンス](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)が設定されていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="78edd-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="78edd-105">Azure AD で操作を実行する権限があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="78edd-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="78edd-106">デバイス登録の設定を管理できるのは、Azure AD のグローバル管理者のみです。</span><span class="sxs-lookup"><span data-stu-id="78edd-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="78edd-107">Azure AD 参加の実装を行うには、「[Azure AD 参加の計画](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78edd-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="78edd-108">Azure AD 参加に関する一般的な問題の解決の詳細については、「[Azure AD 参加に関するよくある質問](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq)」を参照してください。また、Windows 10 Pro デバイスについては、「[Windows 10 Pro マシンで Azure AD に参加できない - アップグレードする必要がある - Microsoftコミュニティ](https://answers.microsoft.com/ja-JP/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78edd-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/ja-JP/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
