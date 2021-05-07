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
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Windows 7 コンピューター上の SharePoint に関する問題

SharePoint または OneDrive での作業中に Windows 7 コンピューターでエラーが発生した場合は、TLS 1.0 /1.1 の非推奨に関連している可能性があります。 詳細については、以下を参照してください。

- [Office 365 および Office 365 GCC での TLS 1.2 の準備](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1 / Windows 8 クライアントでは、TLS1.2 を有効にする必要があります。 詳細については、「[クライアントが TLS 1.2 をサポートしていない場合に、認証エラーが発生する](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)」を参照してください。

- KB3140245 をインストールし、レジストリ値を作成します。 詳細については、「 [Windows の WinHTTP で TLS 1.1 および TLS 1.2 を既定のセキュリティ で保護されたプロトコルとして有効にするための更新プログラム](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)」を参照してください。

- Windows 7 SP1 / Windows 8 クライアントは、最新の TLS 暗号スイートがインストールされていることを確認する必要があります。 詳細については、「[Microsoft Security アドバイザリ 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058)」を参照してください。 


