---
title: DKIM セットアップに関する問題の解決方法
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35085877"
---
# <a name="fix-dkim-setup-issues"></a>DKIM セットアップに関する問題の解決方法

カスタム ドメインの DKIM を有効にする際に問題が発生した場合は、次の手順を使用してください。

- ほとんどの DKIM セットアップの問題は、不適切な DNS レコードに関連しています。 DKIM CNAME レコード (TXT レコード**ではありません**) の書式が正しいことを確認します。 詳細については、この[トピック](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)を参照してください。

- ドメインの DNS ホスティン グサービス (通常はドメイン レジストラー) で DKIM DNS レコードを作成または更新したら、その DNS レコードが伝達されるまで待機します。

- 管理センターで DKIM DNS レコードが作成できない場合は、\<CustomDomain\> を目的のカスタム ドメイン (たとえば、contoso.com) に置き換えて、[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) でコマンド `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` を実行してください。
