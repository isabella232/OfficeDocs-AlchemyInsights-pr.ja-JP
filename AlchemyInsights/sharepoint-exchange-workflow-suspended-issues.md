---
title: SharePoint Online の使用を開始する
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051646"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="2ecbc-102">SharePoint のワークフロー</span><span class="sxs-lookup"><span data-stu-id="2ecbc-102">Workflows in SharePoint</span></span>

<span data-ttu-id="2ecbc-103">SharePoint のワークフローでメールが送信されていない場合、組織が Exchange Online の送信者制限を行っている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2ecbc-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="2ecbc-104">次の項目のいずれかに該当する場合は、「ワークフローは中断されています」エラー メッセージが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2ecbc-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="2ecbc-105">SharePoint Online に、SharePoint 2010 または SharePoint 2013 ワークフロー プラットフォームの種類を使用しているワークフローがあります。</span><span class="sxs-lookup"><span data-stu-id="2ecbc-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="2ecbc-106">ワークフローは、ユーザー設定のメール メッセージを一度に 200 を超えるユーザー、または 1 日に 1 万を超える受信者に送信するか、1 分あたり 30 件を超えるメッセージを送信するように、構成されています。</span><span class="sxs-lookup"><span data-stu-id="2ecbc-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="2ecbc-107">ワークフローを実行すると、電子メールメッセージは送信されず、[内部の状態] が "中断" または "受信者に送信できません" に設定されましたという内容のエラー メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2ecbc-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="2ecbc-108">詳細については、次の[記事](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ecbc-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

