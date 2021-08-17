---
title: メールの転送をセットアップする
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
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a5f165dfae13f179cce7be2a707df072af9bdb3832b938b18e3e023daa756b79
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108525"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a>メールボックスのメールの転送設定を確認する

まず、テナントレベルでメール転送を有効にする必要があります。 メールの転送をメールボックスに設定しても動作しない場合 (**エラー "550 5.7.520 アクセスが拒否されました。お客様の組織では外部転送が許可されていません"** が表示されます) は、「[Microsoft 365 での外部メールの自動転送を制御](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)」を参照してください。

メールボックスのメールの転送設定を確認するのは簡単です。 次の手順に従ってください。
  
> ユーザー メールボックスの場合は、[**ユーザー**] \> [**アクティブなユーザー**] に移動して、転送するメールボックスのユーザーを選択します。[**メール**] タブで、[**メールの転送を管理する**] を選択します。

> 共有メールボックスの場合は、[**グループ**] \> [**共有メールボックス**] に移動して、転送する共有メールボックスを選択します。メールの転送の [**編集**] を選択します。

詳細については、「[Microsoft 365 でメール転送を構成する](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)」を参照してください。
  
ユーザーが自分のメールボックスでメールの転送をセットアップできるようにその手順をユーザーに送信するには、「[Microsoft 365 から別のメール アカウントにメールを転送する](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)」ように指示します。1 つのメール アドレスしか転送できないことに注意してください。ユーザーのグループへの転送をセットアップする必要がある場合は、配布リスト ([**グループ**] の下) を作成して、それにユーザーを追加してから、そのグループへの転送を構成します。
  
退職した従業員がいる場合に、実施すべき推奨手順については、「[Microsoft 365 から元従業員を削除する](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee)」を参照してください。