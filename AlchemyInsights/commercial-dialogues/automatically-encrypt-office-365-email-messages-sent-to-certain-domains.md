---
title: 特定のドメインに送信されたOffice 365のメールメッセージを自動的に暗号化
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751317"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>特定のドメインに送信されたOffice 365のメールメッセージを自動的に暗号化

1. [Exchange 管理センター](https://outlook.office365.com/ecp/) で、**[メール フロー]、[ルール]** の順に選択します。 
2. **[}新規 (+)]** アイコンをクリックし、**[メッセージに Office 365 Message Encryption と権利保護を適用する]** をクリックします。
3. **[名前]** には、*contoso.com に送信されるメッセージを暗号化* など、ルールの名前を入力します。
4. **[このルールを適用]** で、**[受信者]、[ドメインが次の値である]** の順に選択します。 
5. **contoso.com** などのドメイン名を入力します。
6. **追加 (+)** アイコンをクリックし、**[OK]** をクリックします。
7. **[次を実行]** フィールドの横にある **[いずれかを選択]** をクリックします。 
8. **[RMS テンプレート]** のドロップダウン メニューで **[暗号化]** を選択し、**[OK]** をクリックします。 (このオプションが表示されない場合は、ご利用のプランに自動暗号化が含まれていないことを意味します。 ただし、追加することができます。)
9. 省略可能な選択を選びます (この時点でできる省略可能な選択の一覧のうち、多くは簡単にするために既定の設定のままにしておくことができます)。
10. **[保存]** をクリックします。

> [!IMPORTANT]
> いつでも戻ってこのルールを編集することができます。

暗号化のルール作成の詳細については、「[Office 365 でメール メッセージを暗号化するためにメール フロー ルールを定義する](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)」を参照してください。