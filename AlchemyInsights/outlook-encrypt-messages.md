---
title: Web 上の Outlook での S/MIME
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752865"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="2bd49-102">Outlook で電子メールメッセージを暗号化する</span><span class="sxs-lookup"><span data-stu-id="2bd49-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="2bd49-103">Office 365 Message Encryption は、Microsoft Azure Rights Management (Azure RMS) に基づいて構築されています。これは、Azure Information Protection の一部です。</span><span class="sxs-lookup"><span data-stu-id="2bd49-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="2bd49-104">サブスクリプションに Azure Rights Management または Azure Information Protection が含まれている場合は、Rights Management サービスを**手動で有効または無効にする操作**を行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="2bd49-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="2bd49-105">お客様のフィードバックに基づき、Exchange メールフロールールを有効にして、テナント内の特定の種類の機密情報を含む送信電子メールを既定で自動的に暗号化することはなくなります。</span><span class="sxs-lookup"><span data-stu-id="2bd49-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="2bd49-106">代わりに、yourselves を実行する方法について詳細な説明を提供しています。</span><span class="sxs-lookup"><span data-stu-id="2bd49-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="2bd49-107">機密情報を暗号化するためのトランスポートルールを作成する方法について詳しくは、[この記事](https://aka.ms/OmeEtr)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bd49-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="2bd49-108">Outlook on the Web (旧称**owa**) を使用している場合: 電子メールメッセージを作成するときは、[OWA で**保護**する] をクリックするだけです。</span><span class="sxs-lookup"><span data-stu-id="2bd49-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="2bd49-109">これにより、"転送不可" アクセス許可が適用されます。</span><span class="sxs-lookup"><span data-stu-id="2bd49-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="2bd49-110">[**権限の変更**] をクリックし、[**暗号化**] を選択してメッセージを暗号化します。</span><span class="sxs-lookup"><span data-stu-id="2bd49-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="2bd49-111">Outlook**クライアント**を使用している場合: 暗号化されたメッセージを outlook 2013 または2016、あるいは outlook 2016 for Mac から送信するには、[**オプション** > の**権限**] を選択し、必要な保護オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="2bd49-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="2bd49-112">特定の受信者または外部パートナー組織に送信される**すべての電子メールを自動的に暗号化**するには、Exchange 管理センターでメールフロートランスポートルールを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2bd49-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="2bd49-113">詳細な手順については、[このサポート記事](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)で説明されています。</span><span class="sxs-lookup"><span data-stu-id="2bd49-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

