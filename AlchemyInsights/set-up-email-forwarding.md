---
title: メールの転送をセットアップする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: 4ec122967a93f707478e05ac7874cbc884a88c84
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037190"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a>メールボックスのメールの転送設定を確認する

まず、テナント レベルでメールの転送を有効にする必要があります。 メールの転送をメールボックスに設定しても動作しない場合 (**エラー "550 5.7.520 アクセスが拒否されました。組織で外部転送が許可されていません"** が表示されます) は、「[Microsoft 365 での外部メールの自動転送を制御](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)」を参照してください。

メールボックスでメール転送の設定は簡単に確認できます。 次の手順を実行するだけです。
  
> ユーザー メールボックスの場合は、[**ユーザー**] \> [**アクティブなユーザー**] に移動して、転送するメールボックスのユーザーを選択します。[**メール**] タブで、[**メールの転送を管理する**] を選択します。

> 共有メールボックスの場合は、[**グループ**] \> [**共有メールボックス**] に移動して、転送する共有メールボックスを選択します。メールの転送の [**編集**] を選択します。

詳細については、「[Microsoft 365 でメール転送を構成する](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)」を参照してください。
  
ユーザーが自分のメールボックスでメールの転送をセットアップできるように、セットアップ手順をユーザーに送信するには、[Microsoft 365 から別のメール アカウントにメールを転送する](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)ように指示します。 転送は、1 つのメール アドレスに対してのみ可能な点に注意してください。 ユーザーのグループへの転送をセットアップする必要がある場合は、配布リスト ([**グループ**] の下) を作成し、配布リストにユーザーを追加し、そのグループへの転送を構成します。
  
従業員が退職する場合 推奨される手順については、「[Microsoft 365 から元従業員を削除する](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee)」を参照してください。