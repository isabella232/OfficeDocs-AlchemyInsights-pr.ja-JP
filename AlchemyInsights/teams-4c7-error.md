---
title: Teams 4c7 エラー
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/19/2019
ms.locfileid: "40825888"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft Teams の 4c7 エラー

このエラーは、Microsoft Teams でフォーム認証が必要な場合に発生します。 Active Directory フェデレーション サービス (AD FS) を展開した場合、既定では、フォーム認証がイントラネットに対して有効になっていません。 Windows 統合認証に失敗した場合は、フォーム認証を使用してサインインするように求められます。

この問題を解決するには、Active Directory のローカル コピーがあるコンピューターで AD FS Microsoft 管理コンソール (MMC) スナップインを使用して、フォーム認証を有効にします。 これを行うには、次の手順を実行します。 

1. ナビゲーション ウィンドウで、「**認証ポリシー**」を参照します。
2. 詳細ウィンドウの [**アクション**] で、[**グローバル プライマリ認証の編集**] を選択します。
3. [**イントラネット**] タブで、[**フォーム認証**] を選択します。
4. [**OK**] (または [**適用**]) を選択します。