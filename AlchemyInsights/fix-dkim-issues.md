---
title: DKIM セットアップに関する問題の解決方法
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717567"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="f85fa-102">DKIM セットアップに関する問題の解決方法</span><span class="sxs-lookup"><span data-stu-id="f85fa-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="f85fa-103">カスタム ドメインの DKIM を有効にする際に問題が発生した場合は、次の手順を使用してください。</span><span class="sxs-lookup"><span data-stu-id="f85fa-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="f85fa-104">ほとんどの DKIM セットアップの問題は、不適切な DNS レコードに関連しています。</span><span class="sxs-lookup"><span data-stu-id="f85fa-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="f85fa-105">DKIM CNAME レコード (TXT レコード**ではありません**) の書式が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="f85fa-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="f85fa-106">詳細については、この[トピック](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f85fa-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="f85fa-107">ドメインの DNS ホスティン グサービス (通常はドメイン レジストラー) で DKIM DNS レコードを作成または更新したら、その DNS レコードが伝達されるまで待機します。</span><span class="sxs-lookup"><span data-stu-id="f85fa-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="f85fa-108">管理センターで DKIM DNS レコードが作成できない場合は、\<CustomDomain\> を目的のカスタム ドメイン (たとえば、contoso.com) に置き換えて、[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) でコマンド `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` を実行してください。</span><span class="sxs-lookup"><span data-stu-id="f85fa-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
