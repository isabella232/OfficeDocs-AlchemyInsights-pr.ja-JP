---
title: データの場所
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627851"
---
# <a name="data-location"></a>データの場所

Office 365 テナントの場所は管理センターで表示することも、PowerShell を使用して Exchange Online に接続して表示することもできます。


**管理センター:**
1. [管理センター](https://admin.microsoft.com/Adminportal/Home)にログインします。
2. [**設定**]  >  [**組織プロファイル**] の順に選択します。
3. [**データの場所**] で、[**詳細の表示**] を選択します。


**PowerShell:**
1. Windows PowerShell を使用して Exchange Online に接続します。
2. [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) コマンドレットを実行してテナントのプロパティの一覧を表示します。 
3. "OrganizationId" プロパティを確認します。

EXO および SPO のデータの場所がわかれば、[データが格納されている場所](https://products.office.com/where-is-your-data-located)から使用する他のサービスのデータの場所を特定できます。