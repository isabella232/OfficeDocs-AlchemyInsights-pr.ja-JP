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
ms.openlocfilehash: 0515ead28cdfdbdb9529c269b5170b294ab2b120
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543042"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="c1fe9-102">SharePoint で "基になる接続が閉じられました" というエラーが発生する</span><span class="sxs-lookup"><span data-stu-id="c1fe9-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="c1fe9-p101">SharePoint で "基礎となる接続が閉じられました" というエラーが表示される場合、TLS 1.0/1.1 の廃止が関連している可能性があります。詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1fe9-p101">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see these articles:</span></span>

- [<span data-ttu-id="c1fe9-105">Office 365 および Office 365 GCC での TLS 1.2 の準備</span><span class="sxs-lookup"><span data-stu-id="c1fe9-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="c1fe9-106">クライアントが TLS 1.2 をサポートしていない場合に、認証エラーが発生する</span><span class="sxs-lookup"><span data-stu-id="c1fe9-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="c1fe9-107">Windows の WinHTTP で TLS 1.1 および TLS 1.2 を既定のセキュリティ で保護されたプロトコルとして有効にするための更新プログラム</span><span class="sxs-lookup"><span data-stu-id="c1fe9-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="c1fe9-108">ユーザーが Windows 7 を使用している場合は、「[Windows 7 の TLS 暗号スイート](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="c1fe9-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>