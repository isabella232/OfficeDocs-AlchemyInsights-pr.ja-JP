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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207266"
---
# <a name="data-location"></a>データの場所

Office 365 テナントの場所は管理センターで表示することも、PowerShell を使用して Exchange Online に接続して表示することもできます。


**管理センター:**
1. [管理センター](https://admin.microsoft.com/Adminportal/Home)にログインします。
2. [**設定**]  >  [**組織プロファイル**] の順に選択します。
3. [**データの場所**] で、[**詳細の表示**] を選択します。


**PowerShell:**
1. Windows PowerShell を使用して Exchange Online に接続します。
2. [Get-OrganizationalUnit](https://docs.microsoft.com/ja-JP/powershell/module/exchange/active-directory/get-organizationalunit) コマンドレットを実行してテナントのプロパティの一覧を表示します。 
3. "OrganizationId" プロパティを確認します。

EXO および SPO のデータの場所がわかれば、[データが格納されている場所](https://products.office.com/where-is-your-data-located)から使用する他のサービスのデータの場所を特定できます。