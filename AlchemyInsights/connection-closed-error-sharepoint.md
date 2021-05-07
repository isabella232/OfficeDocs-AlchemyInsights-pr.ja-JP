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
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>SharePoint で "基になる接続が閉じられました" というエラーが発生する

SharePoint で "基礎となる接続が閉じられました" というエラーが表示される場合、TLS 1.0/1.1 の廃止が関連している可能性があります。詳細については、次の記事を参照してください。

- [Office 365 および Office 365 GCC での TLS 1.2 の準備](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [クライアントが TLS 1.2 をサポートしていない場合に、認証エラーが発生する](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

ユーザーが Windows 7 を使用している場合は、「[Windows 7 の TLS 暗号スイート](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)」を確認してください。