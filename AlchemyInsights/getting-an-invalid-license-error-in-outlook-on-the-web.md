---
title: 125 Outlook on the web で無効なライセンス エラーが表示される場合
ms.author: daeite
author: daeite
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "125"
- "1600021"
ms.assetid: 6d9947d9-6c92-4ada-b655-8ab2a0c2b66d
ms.openlocfilehash: 357e57d20e3b6f56d3058bc1c782c3da7598520c29c5c29bfba6eec614fc5248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54089265"
---
# <a name="getting-an-invalid-license-error-in-outlook-on-the-web"></a>Outlook on the web で無効なライセンス エラーが表示される場合

Outlook on the web を使用しているときに、**X-OWA-Error: Microsoft.Exchange.Data.Storage.InvalidLicenseException** を含む "**問題が発生しました**" エラーが表示される場合は、Exchange Online ライセンスが正しく割り当てられていないか、最近有効期限が切れています。管理者は、以下の手順に従うことで、ライセンスを割り当てることができます。
  
1. [Microsoft 365 管理センター](https://portal.office.com/adminportal/home#/homepage)を開いて、**[アクティブなユーザー]** で、**[ユーザーの編集]** を選択します。

2. 開いた **[ユーザーの編集]** ページで、ユーザーを選択します。開いた [ユーザーのプロパティ] ページで、**[製品のライセンス]** の **[編集]** をクリックします。

3. 開いた **[製品のライセンス]** ページで、該当する **[場所]** の値を選択し、Exchange Online を含むライセンスを割り当てます (ライセンスを展開して、その詳細を表示します)。完了したら、**[保存]** をクリックします。
