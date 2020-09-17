---
title: Exchange PowerShell と基本認証の廃止
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
- "3500011"
- "4577"
ms.openlocfilehash: f4f0f63112d639101ea9e9d7e9a9c16a32de4cf3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782980"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell と基本認証の廃止

基本認証を使用せずに Exchange Online PowerShell に接続する方法についての最新情報は、[こちらを参照してください](https://aka.ms/exops-docs)。 PowerShell V2 モジュールは基本認証を使用しません。

クライアント コンピューターで基本認証を有効にする必要があることに注意してください。
新しい PowerShell V2 モジュールは、先進認証を使用して、すべての REST ベースの V2 コマンドレットを有効にするための接続を確立します。 V2 コマンドレットに加えて、リモート PowerShell セッションを確立する必要がある古いリモート PowerShell (RPS) コマンドレットにアクセスすることもできます。 Windows コンピューターで RPS セッションを確立するには、モジュールが先進認証メカニズムを使用してサービスを認証する場合でも、クライアント コンピューターで WinRM 基本認証を有効にする必要があります。 WinRM 基本認証パイプラインは、先進認証トークンの転送に使用されます。 クライアント コンピューターで WinRM 基本認証が無効になっている場合、新しい V2 コマンドレットは引き続き機能します (ただし、古い RPS コマンドレットは機能しません)。
