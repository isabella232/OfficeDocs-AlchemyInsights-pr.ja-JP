---
title: Office 365 で特定の メール メッセージを自動的に暗号化
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527922"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Office 365 で特定の メール メッセージを自動的に暗号化

1. [Exchange 管理センター](https://outlook.office365.com/ecp/) で、**[メール フロー]、[ルール]** の順に選択します。 
2. **[}新規 (+)]** アイコンをクリックし、**[メッセージに Office 365 Message Encryption と権利保護を適用する]** をクリックします。
3. **[名前]** には、*すべてのメッセージを暗号化* など、ルールの名前を入力します。
4. **[このルールを適用します]** の **[すべてのメッセージに適用]** を選択します。 
5. **[次を実行]** フィールドの横にある **[いずれかを選択]** をクリックします。 
6. **[RMS テンプレート]** のドロップダウン メニューで **[暗号化]** を選択し、**[OK]** をクリックします。 (このオプションが表示されない場合は、ご利用のプランに自動暗号化が含まれていないことを意味します。 ただし、追加することができます。)
7. **[このルールをセキュリティ レベルで監査]** チェックボックスをオンにして、必要なレベルを選択します。 ご所属の会社で、すべてのメールを暗号化して送信する契約上の義務がある場合は、レベルを **[高]** に設定することをお勧めします。
8. **[このルールのモデルを選択]** で、**[強制]** をクリックします。 
9. 省略可能な選択を選びます (この時点でできる省略可能な選択の一覧のうち、多くは簡単にするために既定の設定のままにしておくことができます)。
10. **[保存]** をクリックします。

> [!IMPORTANT]
> いつでも戻ってこのルールを編集することができます。

暗号化のルール作成の詳細については、「[Office 365 でメール メッセージを暗号化するためにメール フロー ルールを定義する](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)」を参照してください。

