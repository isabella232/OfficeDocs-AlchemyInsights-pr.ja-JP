---
title: SMTP 認証の問題を解決する
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826420"
---
# <a name="solving-smtp-authentication-issues"></a>SMTP 認証の問題を解決する

SMTP メールを送信してクライアントまたはアプリケーションで認証しようとしたときにエラー 5.7.57 または 5.7.3 が発生した場合は、いくつかの点を確認する必要があります。

- 認証済みの SMTP 送信が、テナントまたは使用しようとしているメールボックスで無効になっている可能性があります (両方の設定を確認します)。 詳しくは、「[認証済みのクライアント SMTP 送信を有効または無効にする](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)」をご覧ください。

- テナントで [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) が有効になっているかどうかを確認します。有効になっていると、基本認証 (従来の認証とも呼ばれます。これはユーザー名とパスワードを使用します) を使用した SMTP 認証は失敗します。
