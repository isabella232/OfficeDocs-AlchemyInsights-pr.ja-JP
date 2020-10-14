---
title: Outlook on the web の S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772303"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="67488-102">Outlook でメール メッセージを暗号化する</span><span class="sxs-lookup"><span data-stu-id="67488-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="67488-103">Microsoft 365 Message Encryption は、Azure Information Protection の一部である Microsoft Azure Rights Management (Azure RMS) 上に構築されています。</span><span class="sxs-lookup"><span data-stu-id="67488-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="67488-104">サブスクリプションに Azure Rights Management または Azure Information Protection が含まれている場合は、Rights Management Service を**有効化またはアクティブ化するために手動での操作を行う必要はありません**。</span><span class="sxs-lookup"><span data-stu-id="67488-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="67488-105">お客様からのフィードバックに基づき、特定の種類の機密情報を含む送信メールを自動的に暗号化する Exchange のメール フロー ルールは、テナントで既定で有効化されなくなりました。</span><span class="sxs-lookup"><span data-stu-id="67488-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="67488-106">代わりに、ユーザー自身がこの操作を行うための詳細な手順を提供いたします。</span><span class="sxs-lookup"><span data-stu-id="67488-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="67488-107">機密情報を暗号化するためのトランスポート ルールを作成する方法の詳細については、[こちらの記事](https://aka.ms/OmeEtr)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67488-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="67488-108">Outlook on the Web (以前の **OWA**) を使用している場合: メール メッセージを作成する際に、OWA で [**保護**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="67488-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="67488-109">これにより、"転送不可" のアクセス許可が既定で適用されます。</span><span class="sxs-lookup"><span data-stu-id="67488-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="67488-110">[**アクセス許可の変更**] をクリックし、[**暗号化**] を選択してメッセージの暗号化のみを行います。</span><span class="sxs-lookup"><span data-stu-id="67488-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="67488-111">**Outlook クライアント**を使用している場合: Outlook 2013 または 2016、または Outlook 2016 for Mac から暗号化されたメッセージを送信するには、[**オプション**]  >  [**アクセス権**] を選択し、必要な保護オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="67488-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="67488-112">特定の受信者または外部パートナーの組織に送信される**すべてのメールを自動的に暗号化する**には、Exchange 管理センターでメール フロー トランスポート ルールを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="67488-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="67488-113">詳細な手順については、[このサポート記事](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67488-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

