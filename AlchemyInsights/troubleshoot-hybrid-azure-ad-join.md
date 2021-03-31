---
title: ハイブリッド Azure AD 参加のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401912"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="98ac1-102">ハイブリッド Azure AD 参加のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="98ac1-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="98ac1-103">強く推奨するデバイスが[デバイス登録接続のテスト スクリプト](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)を使用して、システム アカウントでデバイス登録エンド ポイントにアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="98ac1-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="98ac1-104">初めてデバイス登録を設定する場合は、[Azure Active Directory でのデバイス管理の概要](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)を確認して、Azure AD の制御下でデバイスを取得する方法を確認してください。</span><span class="sxs-lookup"><span data-stu-id="98ac1-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="98ac1-105">デバイスを Azure AD に直接登録し、それらを Intune に登録する場合は、[Intune を構成](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)し、最初に[ライセンス](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)を設定していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="98ac1-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="98ac1-106">Azure AD およびオンプレミス AD で操作を実行する権限があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="98ac1-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="98ac1-107">デバイス登録の設定を管理できるのは、Azure AD のグローバル管理者のみです。</span><span class="sxs-lookup"><span data-stu-id="98ac1-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="98ac1-108">さらに、オンプレミスの Active Directory で自動登録を設定する場合は、Active Directory と AD FS (該当する場合) の管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="98ac1-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="98ac1-109">ハイブリッド参加に関する潜在的な問題の解決の詳細については、「ハイブリッド Azure AD 参加をセットアップするための[ハイブリッド参加のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)」を参照してください。Azure AD ポータルを使用したデバイスの管理については、「[ハイブリッド Azure AD に参加した (オンプレミスのドメインに参加した) デバイスのセットアップ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support)」および「[Azure ポータルを使用したデバイスの管理](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98ac1-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="98ac1-110">ハイブリッド Azure Active Directory (AD) 参加に関する一般的な問題を解決するには、「[ハイブリッド Azure AD 参加に関するよくある質問](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="98ac1-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
