---
title: トランスポート ルールを使用した暗号化
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813873"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="674d1-102">トランスポート ルールを使用した暗号化</span><span class="sxs-lookup"><span data-stu-id="674d1-102">Encryption with transport rules</span></span>

<span data-ttu-id="674d1-103">[Exchange 管理センター](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) では、メール フロー ルールで Office Message Encryption (OME) 機能を使用して、メッセージの暗号化をトリガーできます。</span><span class="sxs-lookup"><span data-stu-id="674d1-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="674d1-104">トランスポート ルールの条件で、**[Office 365 Message Encryption および権利保護を適用する]** オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="674d1-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="674d1-105">詳細については、「[暗号化するためのメールフロー ルールを定義する](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="674d1-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="674d1-106">Powershell で、[New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) コマンドレットを使用して、"*ApplyOME*" パラメーターを $true に設定します。</span><span class="sxs-lookup"><span data-stu-id="674d1-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
