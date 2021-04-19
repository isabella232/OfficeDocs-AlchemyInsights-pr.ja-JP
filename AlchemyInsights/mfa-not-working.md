---
title: MFA の問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810489"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA の問題
ユーザーが多要素認証 (MFA) を使用してログインできないかどうかを確認する方法がいくつかあります。

1. 影響を受けるユーザーが Azure Active Directory ポータルでブロックされている可能性があります。 そのような場合は、その特定のユーザーの認証試行が自動的に拒否されます。 [問題を解決するには、この記事の手順を実行してください。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. ユーザーのブロックを解除しても問題が解決しない場合や、ユーザーがブロックされていない場合は、ユーザーの MFA をリセットしてから、登録プロセスを繰り返します。 [この記事の手順に従ってください。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

MFA を初めて有効にして、ユーザーが Outlook や Skype などのブラウザー以外のクライアントにログインできない場合は、O365 サブスクリプションで ADAL (Active Directory 認証ライブラリ) が有効になっていない可能性があります。 この場合は、Exchange Online Powershell に接続して、次のコマンドレットを実行する必要があります: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*