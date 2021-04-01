---
title: Azure Active Directory に参加しているデバイスのシングル サインオン
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
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405849"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="8ea3a-102">Azure Active Directory に参加しているデバイスのシングル サインオン</span><span class="sxs-lookup"><span data-stu-id="8ea3a-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="8ea3a-103">オンプレミスの Active Directory (AD) 環境があり、AD ドメイン参加済みのコンピューターを Azure AD に参加させたい場合、「 ハイブリッド Azure AD 参加」を行うことで実現できます。</span><span class="sxs-lookup"><span data-stu-id="8ea3a-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="8ea3a-104">[方法: ハイブリッド Azure Active Directory 参加の実装計画](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)では、環境にハイブリッド Azure AD 参加を実装するための関連する手順を提供します。</span><span class="sxs-lookup"><span data-stu-id="8ea3a-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="8ea3a-105">Windows Hello for Business を使用して Azure AD に参加しているデバイスをオンプレミスのシングル サインオン用に構成する</span><span class="sxs-lookup"><span data-stu-id="8ea3a-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="8ea3a-106">**プライマリ 更新トークン (PRT) が発行** プライマリ 更新トークン (PRT) は、Windows 10、Windows Server 2016 以降のバージョン、iOS、Android デバイス上の Azure AD 認証の主要な成果物です。</span><span class="sxs-lookup"><span data-stu-id="8ea3a-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="8ea3a-107">これは、Microsoft のファースト パーティ トークン ブローカーに特別に発行される JSON Web トークン (SSO) であり、これらのデバイスで使用されるアプリケーション全体でシングル サインオン (SSO) が有効になります。</span><span class="sxs-lookup"><span data-stu-id="8ea3a-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="8ea3a-108">「[プライマリ リフレッシュ トークンとは?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)」では、Windows 10 デバイスで PRT が発行、使用、保護される方法の詳細を説明しています。</span><span class="sxs-lookup"><span data-stu-id="8ea3a-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="8ea3a-109">**WamDefaultSet: YES および AzureADPrt: YES** これらのフィールドは、デバイスにサインインするときに、ユーザーが Azure AD に対して正常に認証されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8ea3a-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="8ea3a-110">値が [**いいえ**] の場合、次の原因が考えられます。</span><span class="sxs-lookup"><span data-stu-id="8ea3a-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="8ea3a-111">登録時にデバイスに関連付けられている TPM のストレージ キーが正しくありません (管理者特権の実行中に、KeySignTest を確認してください)。</span><span class="sxs-lookup"><span data-stu-id="8ea3a-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="8ea3a-112">代替ログイン ID</span><span class="sxs-lookup"><span data-stu-id="8ea3a-112">Alternate Login ID</span></span>
- <span data-ttu-id="8ea3a-113">HTTP プロキシが見つかりません</span><span class="sxs-lookup"><span data-stu-id="8ea3a-113">HTTP Proxy not found</span></span>

<span data-ttu-id="8ea3a-114">dsregcmd コマンドを使用してデバイスのトラブルシューティングを行う -[SSOの状態](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="8ea3a-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
