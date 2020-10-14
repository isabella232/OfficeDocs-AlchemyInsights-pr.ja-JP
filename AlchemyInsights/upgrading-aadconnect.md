---
title: 932 AADConnect のアップグレード
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806044"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect をアップグレードする

既定では、Azure AD Connect の自動アップグレードが有効になっています。これはユーザーが確実に最新バージョンを実行するために役立ちます。自動アップグレードの設定を確認するには、Azure AD PowerShell で **Get-ADSyncAutoUpgrade** コマンドレットを使用します。コマンドレットは次のいずれかの値を返します。

- **Enabled**: 自動アップグレードが有効になっています。

- **Disabled**: 自動アップグレードが無効になっています。

- **Suspended**: システムが自動アップグレードの受信に対して不適格になっています。この値はシステムによって設定されます。ユーザーが設定することはできません。

詳細については、「[自動アップグレード](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)」を参照してください。

最新バージョンの Azure AD Connect をダウンロードするには、[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) に移動します。
