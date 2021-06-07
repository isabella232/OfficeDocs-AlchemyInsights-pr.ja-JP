---
title: Exchange Online プロトコルの基本認証を有効にする診断
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11392"
- "9006699"
ms.openlocfilehash: 8952aba3dc6b5abcf56776d81eddd9b50db33c7f
ms.sourcegitcommit: d3a739b75d521837660ce151190a7e232e4eeadb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/27/2021
ms.locfileid: "52732068"
---
# <a name="diagnostic-to-enable-basic-authentication-for-exchange-online-protocols"></a><span data-ttu-id="aa047-102">Exchange Online プロトコルの基本認証を有効にする診断</span><span class="sxs-lookup"><span data-stu-id="aa047-102">Diagnostic to enable Basic authentication for Exchange Online protocols</span></span>

<span data-ttu-id="aa047-103">この診断を使用すると、POP3、IMAP4、Exchange ActiveSync、Exchange Web サービス、オフライン アドレス帳、MAPI、RPC、リモート PowerShell などの Exchange Online プロトコルの基本認証を有効にすることができます。これらは、Microsoft が組織に対して最近無効にした可能性があります。</span><span class="sxs-lookup"><span data-stu-id="aa047-103">By using this diagnostic, you can enable Basic authentication for Exchange Online protocols such as POP3, IMAP4, Exchange ActiveSync, Exchange Web Services, Offline Address Book, MAPI, RPC and Remote PowerShell, which Microsoft might have disabled recently for your organization.</span></span> 

<span data-ttu-id="aa047-104">メッセージ センターを介して直接通信を送信して、使用しないため環境内の基本認証を無効にする準備ができている場所をテナントに通知します。これは、関連するセキュリティ リスクから環境を保護するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="aa047-104">We are sending direct communications through Message Center to let tenants know where they're ready to turn off Basic authentication in their environment due to no use, which will help protect their environments from related security risks.</span></span>