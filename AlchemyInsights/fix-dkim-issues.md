---
title: DKIM セットアップに関する問題の解決方法
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945936"
---
# <a name="fix-dkim-setup-issues"></a>DKIM セットアップに関する問題の解決方法

カスタム ドメインの DKIM を有効にする際に問題が発生した場合は、次の手順を使用してください。

- ほとんどの DKIM セットアップの問題は、不適切な DNS レコードに関連しています。 DKIM CNAME レコード (TXT レコード **ではありません**) の書式が正しいことを確認します。 詳細については、この[トピック](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)を参照してください。

- ドメインの DNS ホスティン グサービス (通常はドメイン レジストラー) で DKIM DNS レコードを作成または更新したら、その DNS レコードが伝達されるまで待機します。

- 管理センターで DKIM DNS レコードが作成できない場合は、\<CustomDomain\> を目的のカスタム ドメイン (たとえば、contoso.com) に置き換えて、[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) でコマンド `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` を実行してください。
