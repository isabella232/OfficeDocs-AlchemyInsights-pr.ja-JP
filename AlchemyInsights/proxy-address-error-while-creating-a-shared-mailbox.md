---
title: 共有メールボックスの作成時に発生するプロキシ アドレス エラー
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568295"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>メールボックスまたはメールが有効なその他のオブジェクトの作成時に発生するプロキシ アドレス エラー

メールが有効なオブジェクト (メールボックス、共有メールボックスなど) を作成しようとしたところ、「プロキシ アドレス "SMTP:alias@domain.com" は既に使用されています...」というエラーが表示される場合は、選択したメール アドレスが組織内のメールが有効な別のオブジェクトで既に使用されています。
  
このメール アドレスが指定されているユーザー、グループ、共有メールボックス、またはパブリック フォルダーを検索して、削除するか、メール アドレスを変更する必要があります。 その後、解放されたメール アドレスを使用してメールが有効なオブジェクトを新しく作成できるようになります。 メール アドレスを検索するには、ホームページの [検索] を使用します。 次の Exchange Online PowerShell コマンドを使って検索することもできます。

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
既存のメール アドレスを削除しない場合は、作成しようとしている新しいオブジェクトに対して新しいメール アドレスを選択します。
  