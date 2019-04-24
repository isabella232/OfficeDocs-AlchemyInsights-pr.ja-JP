---
title: 932 AADConnect のアップグレード
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389705"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect をアップグレードする

既定では、Azure AD Connect の自動アップグレードが有効になっています。これはユーザーが確実に最新バージョンを実行するために役立ちます。自動アップグレードの設定を確認するには、Azure AD PowerShell で **Get-ADSyncAutoUpgrade** コマンドレットを使用します。コマンドレットは次のいずれかの値を返します。 

- **Enabled**: 自動アップグレードが有効になっています。

- **Disabled**: 自動アップグレードが無効になっています。

- **Suspended**: システムが自動アップグレードの受信に対して不適格になっています。この値はシステムによって設定されます。ユーザーが設定することはできません。 

詳細については、「[自動アップグレード](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)」を参照してください。

最新バージョンの Azure AD Connect をダウンロードするには、[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) に移動します。
