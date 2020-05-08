---
title: 既定の Yammer ドメインを変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/01/2020
ms.locfileid: "44012663"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>既定の、または主要な Yammer ドメインを変更する

Yammer の URL には、Yammer ネットワークの現在のプライマリ ドメイン名が含まれます。 このドメイン名は、Office 365 または Azure AD で設定されているプライマリ ドメイン名と一致しない可能性があります。 テナントに追加されたカスタム ドメインの数や、Yammer がサポートされている構成 (1 テナント : 1 ネットワーク、または 1 : 1) に基づいて、動作に違いがあります。 [Yammer ドメインおよび Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) の説明書については、こちらを参照してください。

間違ったドメインが表示される最も一般的な理由は、複数の Yammer ネットワークが存在し、統合する必要があることです。 ネットワーク移行ツールを使用して[1つのネットワークに統合](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)することは、重要な第一歩です。 プライマリ ドメインを設定する前にこれを完了します。

**カスタム ドメインはありません**

新しいテナントの場合、テナントからの既定のドメイン (たとえば、fabrikam.onmicrosoft.com) が Yammer に使用されます。 プライマリ ドメインが yammer.com / fabrikam.onmicrosoft.com に設定されます。

**単一のカスタムドメイン**

Yammer では、カスタム ドメイン (fabrikam.com など) が Yammer のプライマリ ドメインとしてテナントから自動的に選択されます。 Yammer.com / fabrikam.com に設定されます。 この変更は、ドメイン同期サービスによって実行され、最大で24時間かかる場合があります。

**複数のカスタムドメイン**

Yammer は、既定のテナント ドメインとは異なるプライマリ ドメインを持つことができます。 複数のカスタム ドメインがあるので、Yammer では、使用可能なドメインから正しいドメインを推測しません。 プライマリドメイン名が選択したプライマリドメインに変更されるようにするには、サポート案件を依頼する必要があります。

**その他のトラブルシューティング情報**

場合によっては、ドメインがテナント間で移動されていて、ドメイン同期サービスが正常に実行されていない可能性があります。 サインインまたはその他の問題に加えて、プライマリドメインが正しくない可能性があります。 この問題を解決するには、Microsoft サポートによる支援を受け、ドメインを正しいネットワークに移動する必要がある場合があります。 特に、ドメイン名のリストが非常に長い場合、このような状況は直接的な支援と解決に時間がかかる可能性があります。 サポート案件を開いて、これらの種類の問題の解決方法をご確認ください。

サポートエージェントを使用している場合は、管理者が管理しているテナントでドメインが検証されます。 ユーザーがテナントに追加されても、DNS によって確認されない場合は、ドメインに関する追加認証の質問を求められることがあります。 ドメインが DNS によって確認され、プロセスが高速化されていることを確認します。
