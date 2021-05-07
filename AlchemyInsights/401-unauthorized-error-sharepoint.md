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
# <a name="401-unauthorized-error-in-sharepoint"></a>SharePoint の 401 Unauthorized エラー

SharePoint で「(401) Unauthorized」というエラーが表示される場合、TLS 1.0/1.1 の非推奨化が関連している可能性があります。詳細については、以下を参照してください。

[Office 365 および Office 365 GCC での TLS 1.2 の準備](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[クライアントが TLS 1.2 をサポートしていない場合に、認証エラーが発生する](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

ユーザーが Windows 7 を使用している場合は、「[Windows 7 の TLS 暗号スイート](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)」を確認してください。