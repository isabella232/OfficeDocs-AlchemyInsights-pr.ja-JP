---
title: 例となる Microsoft Defender for Office 365 フィッシング対策ポリシーはありません。
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751432"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>例となる Microsoft Defender for Office 365 フィッシング対策ポリシーはありません。

これらの設定により、「*ドメインおよびCEO*」と呼ばれるポリシーが有効になります。 このポリシーは、ユーザーとドメインの両方を偽装から保護し、ドメイン内のユーザーが受信するメールにポリシーを適用します。 最初に、パッケージを作成するために、次の情報を入力します。

- **名前**: ドメインと CEO の **説明**: CEO とお客様のドメインが偽装されていないことを確認します。
  **適用となる対象**: [**受信者のドメインは**] を選択します。 [**これらの内のいずれか**] で、[**選択**] を選択し、それからドメインを選択します。 **[+ 追加]** を選択します。 リスト内のドメイン名(*contoso.com* など)の横にあるチェックボックスを選択し、[**追加**] を選択します。 [**完了**] を選択します。
- ポリシーを作成したら、次のオプションを使用してポリシーを微調整できます。
  - **保護するユーザーを追加する:** この例では、少なくとも CEO のメール アドレスを追加します。
  - **保護するドメインを追加する**: CEO のオフィスを含む組織のドメインを追加します。
  - **アクションの選択**: **偽装されたユーザーによってメールが送信された場合** は、[**メッセージを別のメール アドレスにリダイレクトする**] を選び、セキュリティ管理者のメール アドレス ( *securityadmin@contoso.com* など) を入力します。 **偽装されたドメイン アカウントによってメールを送信された場合** は、[**メッセージを検疫**] を選択します。
  - **メールボックス インテリジェンス**: 規定では、新しいフィッシング対策ポリシーの作成時にはこのオプションが選択されています。 最適な結果が得られるように、この設定は **[オン]** のままにしておいてください。
  - **信頼できる差出人とドメインを追加する:** この例では、上書きを定義しないでください。
- 設定を確認したら、必要に応じて [**このポリシーを作成する**] または [**保存する**] を選択します。

詳細については、「[Microsoft 365 のフィッシング詐欺対策ポリシー](https://go.microsoft.com/fwlink/?linkid=2092235)」をご覧ください。
