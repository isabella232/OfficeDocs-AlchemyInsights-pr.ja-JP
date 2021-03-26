---
title: エラー コード AADSTS650056 のトラブルシューティング
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
- "9803"
- "9005744"
ms.openlocfilehash: 945be2b496b98937bfae6d1f573162d1f2ebb4b6
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038347"
---
# <a name="troubleshoot-error-code-aadsts650056"></a><span data-ttu-id="0613e-102">エラー コード AADSTS650056 のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="0613e-102">Troubleshoot error code AADSTS650056</span></span>

<span data-ttu-id="0613e-103">AADSTS650056 エラーを解決するには、次の推奨される手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="0613e-103">To resolve AADSTS650056 error, perform the below recommended step.</span></span>

<span data-ttu-id="0613e-104">**AADSTS65005**: MisconfiguredApplication - アプリの必須リソース アクセス リストに、リソースによって検出可能なアプリが含まれていません。または、必須リソース アクセス リストで指定されていないリソースへのアクセスをクライアント アプリが要求したか、Graph サービスから無効な要求が返されたか、リソースが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="0613e-104">**AADSTS65005**: MisconfiguredApplication - The app required resource access list does not contain apps discoverable by the resource or The client app has requested access to resource, which was not specified in its required resource access list or Graph service returned bad request or resource not found.</span></span> <span data-ttu-id="0613e-105">アプリが SAML をサポートしている場合、間違った識別子 (エンティティ) でアプリを構成しているおそれがあります。</span><span class="sxs-lookup"><span data-stu-id="0613e-105">If the app supports SAML, you may have configured the app with the wrong Identifier (Entity).</span></span>

<span data-ttu-id="0613e-106">詳細については、エラー [AADSTS650056](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts650056-misconfigured-app) に関するトラブルシューティング記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0613e-106">For more information, see the troubleshooting article for error [AADSTS650056](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts650056-misconfigured-app).</span></span>
