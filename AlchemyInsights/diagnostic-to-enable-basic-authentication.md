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
ms.openlocfilehash: 25979df257d0534709f610b4d1547c52aeb269053c3d15a38969f15223b59e04
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993610"
---
# <a name="diagnostic-to-enable-basic-authentication-for-exchange-online-protocols"></a>Exchange Online プロトコルの基本認証を有効にする診断

この診断を使用すると、POP3、IMAP4、Exchange ActiveSync、Exchange Web サービス、オフライン アドレス帳、MAPI、RPC、リモート PowerShell などの Exchange Online プロトコルの基本認証を有効にすることができます。これらは、Microsoft が組織に対して最近無効にした可能性があります。 

メッセージ センターを介して直接通信を送信して、使用しないため環境内の基本認証を無効にする準備ができている場所をテナントに通知します。これは、関連するセキュリティ リスクから環境を保護するのに役立ちます。