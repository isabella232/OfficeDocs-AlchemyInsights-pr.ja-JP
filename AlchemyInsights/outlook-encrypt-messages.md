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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772303"
---
# <a name="encrypt-email-messages-in-outlook"></a>Outlook でメール メッセージを暗号化する

Microsoft 365 Message Encryption は、Azure Information Protection の一部である Microsoft Azure Rights Management (Azure RMS) 上に構築されています。 サブスクリプションに Azure Rights Management または Azure Information Protection が含まれている場合は、Rights Management Service を**有効化またはアクティブ化するために手動での操作を行う必要はありません**。

お客様からのフィードバックに基づき、特定の種類の機密情報を含む送信メールを自動的に暗号化する Exchange のメール フロー ルールは、テナントで既定で有効化されなくなりました。 代わりに、ユーザー自身がこの操作を行うための詳細な手順を提供いたします。 機密情報を暗号化するためのトランスポート ルールを作成する方法の詳細については、[こちらの記事](https://aka.ms/OmeEtr)を参照してください。

- Outlook on the Web (以前の **OWA**) を使用している場合: メール メッセージを作成する際に、OWA で [**保護**] をクリックします。 これにより、"転送不可" のアクセス許可が既定で適用されます。 [**アクセス許可の変更**] をクリックし、[**暗号化**] を選択してメッセージの暗号化のみを行います。

- **Outlook クライアント**を使用している場合: Outlook 2013 または 2016、または Outlook 2016 for Mac から暗号化されたメッセージを送信するには、[**オプション**]  >  [**アクセス権**] を選択し、必要な保護オプションを選択します。

- 特定の受信者または外部パートナーの組織に送信される**すべてのメールを自動的に暗号化する**には、Exchange 管理センターでメール フロー トランスポート ルールを作成する必要があります。 詳細な手順については、[このサポート記事](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)を参照してください。

