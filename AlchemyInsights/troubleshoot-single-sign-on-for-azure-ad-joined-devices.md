---
title: Azure AD に参加しているデバイスのシングル サインオンのトラブルシューティング
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038283"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="bb613-102">Azure AD に参加しているデバイスのシングル サインオンのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="bb613-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="bb613-103">オンプレミスの Active Directory (AD) 環境があり、AD ドメイン参加済みのコンピューターを Azure AD に参加させたい場合、「 ハイブリッド Azure AD 参加」を行うことで実現できます。</span><span class="sxs-lookup"><span data-stu-id="bb613-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="bb613-104">[方法: ハイブリッド Azure Active Directory 参加の実装計画](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)では、環境にハイブリッド Azure AD 参加を実装するための関連する手順を提供します。</span><span class="sxs-lookup"><span data-stu-id="bb613-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="bb613-105">詳細については、「[Windows Hello for Business を使用して Azure AD に参加しているデバイスをオンプレミスのシングル サインオン用に構成する](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb613-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="bb613-106">**プライマリ 更新トークン (PRT) 問題**</span><span class="sxs-lookup"><span data-stu-id="bb613-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="bb613-107">プライマリ 更新トークン (PRT) は、Windows 10、Windows Server 2016 以降のバージョン、iOS、Android デバイス上の Azure AD 認証の主要な成果物です。</span><span class="sxs-lookup"><span data-stu-id="bb613-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="bb613-108">これは、Microsoft のファースト パーティ トークン ブローカーに特別に発行される JSON Web トークン (SSO) であり、これらのデバイスで使用されるアプリケーション全体でシングル サインオン (SSO) が有効になります。</span><span class="sxs-lookup"><span data-stu-id="bb613-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="bb613-109">Windows 10 デバイスで PRT が発行、使用、保護される方法の詳細については、「[プライマリ リフレッシュ トークンとは](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)」を参照してください。 </span><span class="sxs-lookup"><span data-stu-id="bb613-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="bb613-110">**WamDefaultSet: YES および AzureADSet: YES**</span><span class="sxs-lookup"><span data-stu-id="bb613-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="bb613-111">これらのフィールドは、デバイスにサインインするときに、ユーザーが Azure AD に対して正常に認証されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bb613-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="bb613-112">値が [**いいえ**] の場合、次の原因が考えられます。</span><span class="sxs-lookup"><span data-stu-id="bb613-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="bb613-113">登録時にデバイスに関連付けられている TPM のストレージ キーが正しくありません (管理者特権の実行中に、KeySignTest を確認してください)</span><span class="sxs-lookup"><span data-stu-id="bb613-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="bb613-114">代替ログイン ID</span><span class="sxs-lookup"><span data-stu-id="bb613-114">Alternate Login ID</span></span>
- <span data-ttu-id="bb613-115">HTTP プロキシが見つかりません</span><span class="sxs-lookup"><span data-stu-id="bb613-115">HTTP Proxy not found</span></span>

<span data-ttu-id="bb613-116">dsregcmd コマンドを使用してデバイスのトラブルシューティングを行うには、「[SSOの状態](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb613-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
