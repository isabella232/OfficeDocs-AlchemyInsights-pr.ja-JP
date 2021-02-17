---
title: レプリカ セット
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8265"
ms.openlocfilehash: 7b6d614fddfcb5722e426b520f1c0d6c539c7f33
ms.sourcegitcommit: 9400cd853b7a5a81f6f5a1ad9601fef37c18bcae
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2021
ms.locfileid: "50254941"
---
# <a name="replica-set"></a>レプリカ セット

AADDS は管理対象ドメインとも呼ばれます。 実際には、バックエンドによって実行および保守される 2 つのドメイン コントローラーです。 2 つの DC には、メイン DC とレプリケーション DC が 1 つずつ含まれます。 AADDS (管理対象ドメイン) でのバックアップは、Azure プラットフォームによって管理される自動プロセスです。 管理対象ドメインに問題が発生した場合は、Azure サポートがバックアップからの復元を支援します。

仮想ネットワーク内で各レプリカ セットを作成します。 各仮想ネットワークは、管理対象ドメインのレプリカセットをホストする他のすべての仮想ネットワークとピアリングする必要があります。 この構成では、ディレクトリ レプリケーションをサポートするメッシュ ネットワーク トポロジが作成されます。 各レプリカ セットが異なる仮想サブネット内にある場合、仮想ネットワークは複数のレプリカ セットをサポートできます。

レプリカ セットの詳細については、「[レプリカ セットの概念](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)」を参照してください。
