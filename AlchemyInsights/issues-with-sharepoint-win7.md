---
title: Windows 7 コンピューター上の SharePoint に関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125842"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="fa170-102">Windows 7 コンピューター上の SharePoint に関する問題</span><span class="sxs-lookup"><span data-stu-id="fa170-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="fa170-103">SharePoint または OneDrive での作業中に Windows 7 コンピューターでエラーが発生した場合は、TLS 1.0 /1.1 の非推奨に関連している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fa170-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="fa170-104">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa170-104">For more information, see:</span></span>

- [<span data-ttu-id="fa170-105">Office 365 および Office 365 GCC での TLS 1.2 の準備</span><span class="sxs-lookup"><span data-stu-id="fa170-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="fa170-106">Windows 7 SP1 / Windows 8 クライアントでは、TLS1.2 を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa170-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="fa170-107">詳細については、「[クライアントが TLS 1.2 をサポートしていない場合に、認証エラーが発生する](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa170-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="fa170-108">KB3140245 をインストールし、レジストリ値を作成します。</span><span class="sxs-lookup"><span data-stu-id="fa170-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="fa170-109">詳細については、「 [Windows の WinHTTP で TLS 1.1 および TLS 1.2 を既定のセキュリティ で保護されたプロトコルとして有効にするための更新プログラム](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa170-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="fa170-110">Windows 7 SP1 / Windows 8 クライアントは、最新の TLS 暗号スイートがインストールされていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa170-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="fa170-111">詳細については、「[Microsoft Security アドバイザリ 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa170-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


