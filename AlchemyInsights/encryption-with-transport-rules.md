---
title: トランスポート ルールを使用した暗号化
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784348"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="b0a99-102">トランスポート ルールを使用した暗号化</span><span class="sxs-lookup"><span data-stu-id="b0a99-102">Encryption with transport rules</span></span>

<span data-ttu-id="b0a99-103">[Exchange 管理センター](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) では、メール フロー ルールで Office Message Encryption (OME) 機能を使用して、メッセージの暗号化をトリガーできます。</span><span class="sxs-lookup"><span data-stu-id="b0a99-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="b0a99-104">トランスポート ルールの条件で、**[Office 365 Message Encryption および権利保護を適用する]** オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="b0a99-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="b0a99-105">詳細については、「[暗号化するためのメールフロー ルールを定義する](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0a99-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="b0a99-106">Powershell で、[New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) コマンドレットを使用して、"*ApplyOME*" パラメーターを $true に設定します。</span><span class="sxs-lookup"><span data-stu-id="b0a99-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
