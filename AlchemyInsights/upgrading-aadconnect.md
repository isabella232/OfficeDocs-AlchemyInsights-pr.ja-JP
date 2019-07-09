---
title: 932 AADConnect のアップグレード
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365906"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect をアップグレードする

既定では、Azure AD Connect の自動アップグレードが有効になっています。これはユーザーが確実に最新バージョンを実行するために役立ちます。自動アップグレードの設定を確認するには、Azure AD PowerShell で **Get-ADSyncAutoUpgrade** コマンドレットを使用します。コマンドレットは次のいずれかの値を返します。

- **Enabled**: 自動アップグレードが有効になっています。

- **Disabled**: 自動アップグレードが無効になっています。

- **Suspended**: システムが自動アップグレードの受信に対して不適格になっています。この値はシステムによって設定されます。ユーザーが設定することはできません。

詳細については、「[自動アップグレード](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)」を参照してください。

最新バージョンの Azure AD Connect をダウンロードするには、[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) に移動します。
