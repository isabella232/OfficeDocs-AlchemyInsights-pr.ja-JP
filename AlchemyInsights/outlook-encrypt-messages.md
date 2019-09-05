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
# <a name="encrypt-email-messages-in-outlook"></a>Outlook で電子メールメッセージを暗号化する

Office 365 Message Encryption は、Microsoft Azure Rights Management (Azure RMS) に基づいて構築されています。これは、Azure Information Protection の一部です。 サブスクリプションに Azure Rights Management または Azure Information Protection が含まれている場合は、Rights Management サービスを**手動で有効または無効にする操作**を行う必要はありません。

お客様のフィードバックに基づき、Exchange メールフロールールを有効にして、テナント内の特定の種類の機密情報を含む送信電子メールを既定で自動的に暗号化することはなくなります。 代わりに、yourselves を実行する方法について詳細な説明を提供しています。 機密情報を暗号化するためのトランスポートルールを作成する方法について詳しくは、[この記事](https://aka.ms/OmeEtr)を参照してください。

- Outlook on the Web (旧称**owa**) を使用している場合: 電子メールメッセージを作成するときは、[OWA で**保護**する] をクリックするだけです。 これにより、"転送不可" アクセス許可が適用されます。 [**権限の変更**] をクリックし、[**暗号化**] を選択してメッセージを暗号化します。

- Outlook**クライアント**を使用している場合: 暗号化されたメッセージを outlook 2013 または2016、あるいは outlook 2016 for Mac から送信するには、[**オプション** > の**権限**] を選択し、必要な保護オプションを選択します。

- 特定の受信者または外部パートナー組織に送信される**すべての電子メールを自動的に暗号化**するには、Exchange 管理センターでメールフロートランスポートルールを作成する必要があります。 詳細な手順については、[このサポート記事](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)で説明されています。

