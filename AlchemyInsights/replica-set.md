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
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110685"
---
# <a name="replica-set"></a>レプリカ セット

AADDS は管理対象ドメインとも呼ばれます。 実際には、バックエンドによって実行および保守される 2 つのドメイン コントローラーです。 2 つの DC には、メイン DC とレプリケーション DC が 1 つずつ含まれます。 AADDS (管理対象ドメイン) でのバックアップは、Azure プラットフォームによって管理される自動プロセスです。 管理対象ドメインに問題が発生した場合は、Azure サポートがバックアップからの復元を支援します。

仮想ネットワーク内で各レプリカ セットを作成します。 各仮想ネットワークは、管理対象ドメインのレプリカセットをホストする他のすべての仮想ネットワークとピアリングする必要があります。 この構成では、ディレクトリ レプリケーションをサポートするメッシュ ネットワーク トポロジが作成されます。 各レプリカ セットが異なる仮想サブネット内にある場合、仮想ネットワークは複数のレプリカ セットをサポートできます。

レプリカ セットの詳細については、「[レプリカ セットの概念](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)」を参照してください。
