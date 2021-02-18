---
title: デバイスの書き戻し
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2021
ms.locfileid: "50257023"
---
# <a name="device-writeback"></a><span data-ttu-id="55ecf-102">デバイスの書き戻し</span><span class="sxs-lookup"><span data-stu-id="55ecf-102">Device Writeback</span></span>

<span data-ttu-id="55ecf-103">デバイスの書き戻しは、次のようなシナリオで使用します。</span><span class="sxs-lookup"><span data-stu-id="55ecf-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="55ecf-104">[ハイブリッド証明書信頼の展開を使用した Windows Hello for Business ](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)を有効にします。</span><span class="sxs-lookup"><span data-stu-id="55ecf-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="55ecf-105">ADFS (2012 R2 以降) で保護されたアプリケーション (証明書利用者の信頼) へのデバイスに基づく条件付きアクセスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="55ecf-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="55ecf-106">デバイスの書き戻しには、Azure AD Premium のサブスクリプションが必要です。</span><span class="sxs-lookup"><span data-stu-id="55ecf-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="55ecf-107">これにより、セキュリティが強化され、アプリケーションへのアクセスが信頼されたデバイスに対してのみ許可されることが保証されます。</span><span class="sxs-lookup"><span data-stu-id="55ecf-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="55ecf-108">条件付きアクセスの詳細については、「[条件付きアクセス ポリシーを使用したリスクの管理](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)」と「[Azure Active Directory Device Registration を使用したオンプレミスの条件付きアクセスの設定](https://docs.microsoft.com/azure/active-directory/devices/overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55ecf-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="55ecf-109">デバイスの書き戻しの有効化に関する詳細については、「[デバイスの書き戻しを有効にする](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55ecf-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
