---
title: エラー autologon.microsoftazuread-sso.com:443 のため Teams にログインできない
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2020
ms.locfileid: "42935330"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="03dee-102">エラー autologon.microsoftazuread-sso dot com:443 のため Teams にログインできない</span><span class="sxs-lookup"><span data-stu-id="03dee-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="03dee-103">シームレス SSO が O365 認証として有効な場合、URL "autologon.microsoftazuread-sso.com" をイントラネット サイトに追加しなければならないことがあります。</span><span class="sxs-lookup"><span data-stu-id="03dee-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="03dee-104">信頼済みサイトに既に追加してあり、シームレス SSO を使用している場合には、信頼済みサイトから削除しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="03dee-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="03dee-105">[シームレス SSO トラブルシューティングのチェックリスト](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="03dee-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="03dee-106">次の手順を使用して、URL をイントラネット サイトの一覧に追加します。</span><span class="sxs-lookup"><span data-stu-id="03dee-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="03dee-107">**[スタート]** ボタンをクリックして、Internet Explorer を開きます。</span><span class="sxs-lookup"><span data-stu-id="03dee-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="03dee-108">検索ボックスに Internet Explorer と入力し、結果の一覧で **Internet Explorer** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="03dee-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="03dee-109">**[ツール]**、**[インターネット オプション]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="03dee-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="03dee-110">**[セキュリティ]** タブをクリックします。</span><span class="sxs-lookup"><span data-stu-id="03dee-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="03dee-111">**[ローカル イントラネット]**、**[サイト]** ボタン、**[詳細設定]** ボタンの順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="03dee-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="03dee-112">Web サイト URL を入力して、**[追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="03dee-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="03dee-113">完了したら、**[閉じる]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="03dee-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="03dee-114">詳細については、[O365 のシームレス SSO の展開に関する資料](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (手順 3 の URL をイントラネット サイトに追加するためのポリシー ベースのプロセスを含め) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03dee-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
