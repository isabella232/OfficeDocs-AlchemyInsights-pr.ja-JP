---
title: SharePoint で "基になる接続が閉じられました" というエラーが発生する
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233431"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="9feda-102">SharePoint で "基になる接続が閉じられました" というエラーが発生する</span><span class="sxs-lookup"><span data-stu-id="9feda-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="9feda-p101">SharePoint で "基礎となる接続が閉じられました" というエラーが表示される場合、TLS 1.0/1.1 の廃止が関連している可能性があります。詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9feda-p101">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see these articles:</span></span>

- [<span data-ttu-id="9feda-105">Office 365 および Office 365 GCC での TLS 1.2 の準備</span><span class="sxs-lookup"><span data-stu-id="9feda-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [<span data-ttu-id="9feda-106">クライアントが TLS 1.2 をサポートしていない場合に、認証エラーが発生する</span><span class="sxs-lookup"><span data-stu-id="9feda-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="9feda-107">ユーザーが Windows 7 を使用している場合は、「[Windows 7 の TLS 暗号スイート](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="9feda-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>