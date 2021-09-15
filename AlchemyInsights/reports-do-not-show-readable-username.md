---
title: Microsoft 365 管理センターのレポートに読み取り可能なユーザー名が表示されない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327819"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Microsoft 365 管理センターのレポートに読み取り可能なユーザー名が表示されない

Microsoft 365 管理センターのレポートにはユーザー名は表示されませんが、代わりに B2BC6C15BB9FCDEA71E5CD302D228CC8 などのアルファ数値が表示されます。

これは予想される動作であり、メッセージ センター (MC275344、2021 年 8 月 3 日公開) で伝達されています。 

グローバル管理者は、組織のプライバシー設定で許可されている場合、テナントのこの変更を元に戻し、識別可能なユーザー情報を表示できます。テナントの変更を元に戻すには:

1. 管理センターで、**[設定]** > **[組織の設定]** > [**[サービス]**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) の順に移動し、**[レポート]** を選択します。 
1. **[ユーザー情報の表示方法の選択]** で、**[レポートに識別可能なユーザー情報を表示する]** を選択し、レポートを再実行します。