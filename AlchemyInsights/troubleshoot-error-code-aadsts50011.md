---
title: エラー コード AADSTS50011 のトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038349"
---
# <a name="troubleshoot-error-code-aadsts50011"></a><span data-ttu-id="e6e17-102">エラー コード AADSTS50011 のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="e6e17-102">Troubleshoot error code AADSTS50011</span></span>

<span data-ttu-id="e6e17-103">AADSTS50011 エラーを解決するには、下記の推奨手順を実行してください。</span><span class="sxs-lookup"><span data-stu-id="e6e17-103">To resolve AADSTS50011 error, perform the recommended step described below.</span></span>

<span data-ttu-id="e6e17-104">**AADSTS50011**: InvalidReplyTo - 返信アドレスが不足している、正しく構成されていない、またはアプリに構成されている返信アドレスと一致しません。</span><span class="sxs-lookup"><span data-stu-id="e6e17-104">**AADSTS50011**: InvalidReplyTo - The reply address is missing, misconfigured, or does not match reply addresses configured for the app.</span></span>

<span data-ttu-id="e6e17-105">解決方法として、この不足している返信アドレスを Azure Active Directory (AD) アプリに追加するか、AD でアプリケーションを管理するアクセス許可を持つユーザーにこの処理を依頼します。</span><span class="sxs-lookup"><span data-stu-id="e6e17-105">As a resolution ensure to add this missing reply address to the Azure Active Directory (AD) app or have someone with the permissions to manage your application in AD do this for you.</span></span> <span data-ttu-id="e6e17-106">詳細については、エラー [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch) に関するトラブルシューティング記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e6e17-106">For more information, see the troubleshooting article for error [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span></span>