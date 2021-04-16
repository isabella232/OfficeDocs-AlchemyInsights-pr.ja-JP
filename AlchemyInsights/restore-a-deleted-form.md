---
title: 削除されたフォームを復元する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 48018accc23a504c34b5469c198d6f29929d25c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809480"
---
# <a name="restore-a-deleted-form"></a>削除されたフォームを復元する

Microsoft Forms のフォームを誤って削除してしまった場合は、フォームを復元することができます。 削除されたフォームの所有者として Microsoft Forms にサインインします。 [**ごみ箱**] を選択してから、回復するフォームを選択し、[**復元**] を選択します。 復元が完了したら、[**フォームに戻る**] ページの矢印を選択します。

フォームの所有者のみが復元できます。 フォーム所有者のアカウントが無効になっているか、テナントから削除されている場合、グローバル管理者のみがフォームを回復できます。 グローバル管理者が復元を実行するには、Forms ライセンスが必要です。 ユーザー アカウントが無効になっているか、テナントから削除されてから 30 日以内に作成されたフォームのみを復元できます。

テナントのグローバル管理者であり、削除または無効化されたアカウントでフォームを復元する場合は、次の URL **https://forms.office.com/Pages/delegatepage.aspx?originalowner=[メール アドレス]** で [メール アドレス] を削除または無効化されたユーザーのメール アドレスに置き換えます。たとえば、メール アドレスが johndoe@contoso.com の場合、URL は **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** のようになります。 

ユーザーの削除したフォームにアクセスしたら、移動するフォームを選択し、[**その他のフォームのアクション**] > [**移動**] の順に選択します。

削除され、ユーザーが組織から削除されたフォームを復元したい場合、グローバル管理者はユーザーを復元し、そのユーザーのパスワードをリセットしてからそのユーザーとしてログインしている間、別のアクティブなユーザーにフォームを移動することができます。 