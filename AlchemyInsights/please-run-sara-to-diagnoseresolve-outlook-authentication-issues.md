---
title: 182 Outlook の認証の問題を診断および解決するには、SaRA を実行してください
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "182"
- "1800012"
ms.assetid: a3a5ea91-6989-4616-9290-c7b24484e8c8
ms.openlocfilehash: e14042fa80be802e646db4e30cd3d5b69b81a1d3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43765536"
---
# <a name="use-sara-to-diagnose-and-resolve-outlook-authentication-issues"></a><span data-ttu-id="cb81d-102">SaRA を使用して Outlook の認証の問題を診断および解決する</span><span class="sxs-lookup"><span data-stu-id="cb81d-102">Use SaRA to diagnose and resolve Outlook authentication issues</span></span>

<span data-ttu-id="cb81d-103">**メモ**: 組織の[セキュリティの既定値群](https://aka.ms/securitydefaults)が有効になっているかどうかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="cb81d-103">**Note**: Please check to see whether [security defaults](https://aka.ms/securitydefaults) is enabled for your organization.</span></span> <span data-ttu-id="cb81d-104">2019 年 10 月 21 日以降にテナントが作成され、Outlook からパスワードの入力を繰り返し求められる場合は、テナントで**セキュリティの既定値群**が有効になっている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="cb81d-104">If your tenant was created after October 21st, 2019 and your Outlook is repeatedly asking you for a password, you may have **security defaults** enabled in your tenant.</span></span>

<span data-ttu-id="cb81d-p102">Outlook からパスワードの入力を引き続き要求される場合、"[Outlook で何度もパスワードの入力を要求されます](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy)" 診断ツールを使用してそのマシンでのトラブルシューティングを行うことを強くお勧めします。この [SaRA](https://diagnostics.office.com/#/) 診断ツールは、自動チェックを行い、検出された問題に対応するのにユーザーが使用できる解決方法を返します。</span><span class="sxs-lookup"><span data-stu-id="cb81d-p102">We highly recommend you use the [Outlook keeps asking for my password](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostic on the affected machine to troubleshoot issues where Outlook continually prompts for a password. This [SaRA](https://diagnostics.office.com/#/) diagnostic does automated checks and returns possible solutions for you to use to address any detected issues.</span></span>
