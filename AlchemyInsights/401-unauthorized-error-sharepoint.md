---
title: SharePoint の 401 Unauthorized エラー
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233508"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="a489e-102">SharePoint の 401 Unauthorized エラー</span><span class="sxs-lookup"><span data-stu-id="a489e-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="a489e-p101">SharePoint で「(401) Unauthorized」というエラーが表示される場合、TLS 1.0/1.1 の非推奨化が関連している可能性があります。詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a489e-p101">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see:</span></span>

[<span data-ttu-id="a489e-105">Office 365 および Office 365 GCC での TLS 1.2 の準備</span><span class="sxs-lookup"><span data-stu-id="a489e-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[<span data-ttu-id="a489e-106">クライアントが TLS 1.2 をサポートしていない場合に、認証エラーが発生する</span><span class="sxs-lookup"><span data-stu-id="a489e-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="a489e-107">ユーザーが Windows 7 を使用している場合は、「[Windows 7 の TLS 暗号スイート](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="a489e-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>