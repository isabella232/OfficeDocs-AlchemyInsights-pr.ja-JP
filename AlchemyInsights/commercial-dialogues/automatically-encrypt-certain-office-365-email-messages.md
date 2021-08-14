---
title: 特定の Office 365 メール メッセージを自動的に暗号化
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
ms.openlocfilehash: 8ae1c6853f41790efc3b24a9dc696bccf8385967d8c9219a1200e287e6ce32a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53949572"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>特定の Office 365 メール メッセージを自動的に暗号化

ユーザーが特定の外部ユーザーや組織に送信するメッセージを自動的に暗号化することができます。 これを実現するには、以下の手順を実行します。

1. [Exchange 管理センター](https://outlook.office365.com/ecp/) で、**[メール フロー]、[ルール]** の順に選択します。 
2. **[}新規 (+)]** アイコンをクリックし、**[メッセージに Office 365 Message Encryption と権利保護を適用する]** をクリックします。
3. **[名前]** には、*DrToniRamos@gmail.com に送信されるメッセージを暗号化* など、ルールの名前を入力します。
4. **[このルールを適用]** で、**[受信者]、[この人物である]** の順に選択します。 
5. **[メンバーの選択]** ウィンドウで、暗号化ルールを適用するユーザーの名前を選択し、**[追加]** をクリックします。 
6. ユーザーの追加が完了したら、[**OK**] をクリックします。
7. **[次を実行]** フィールドの横にある **[いずれかを選択]** をクリックします。 
8. **[RMS テンプレート]** のドロップダウン メニューで **[暗号化]** を選択し、**[OK]** をクリックします。 (このオプションが表示されない場合は、ご利用のプランに自動暗号化が含まれていないことを意味します。 ただし、追加することができます。)
9. 省略可能な選択を選びます (この時点でできる省略可能な選択の一覧のうち、多くは簡単にするために既定の設定のままにしておくことができます)。
10. **[保存]** をクリックします。

> [!IMPORTANT]
> いつでも戻ってこのルールを編集することができます。

OME のメール フロー ルールの作成の手順については、「[Office 365 でメール メッセージを暗号化するためにメール フロー ルールを定義する](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)」を参照してください。

