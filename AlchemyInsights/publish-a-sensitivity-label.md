---
title: 秘密度ラベル用に暗号化を構成する方法
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11015"
- "9000181"
ms.openlocfilehash: 7b9025092c154f2734f74dc547de877e70caac2e
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475222"
---
# <a name="how-to-publish-a-sensitivity-label"></a>秘密度ラベル用に暗号化を構成する方法

1. Microsoft 365 コンプライアンス センター > **Information Protection** > **ラベル ポリシー** に移動します。

1. **[+ ラベルの発行]** を選択して、[新しい秘密度ラベル] ウィザードを起動します。

1. [**発行する秘密度ラベルの選択**] をクリックします。 アプリとサービスで使用するラベルを選択し、[**追加**] を選択します。

    **重要**: サブラベルを選択する場合は、必ず親ラベルも選択してください。

1. 選択したラベルを確認します。 変更を加えるには、[**編集**] を選択します。 それ以外の場合は、[**次へ**] を選択します。

1. 指示に従ってポリシー設定を構成します。

1. 異なるユーザーや場所に対して、異なるポリシー設定が必要な場合は、次の手順を繰り返します。 たとえば、ユーザーのグループにラベルを追加したり、ユーザーのサブセットに別の既定のラベルを作成したりできます。

1. 複数のラベル ポリシーを作成すると、ユーザーまたは場所の競合が発生することがあります。ポリシーの順序を確認し、必要に応じてこれらを上下に移動します。 ラベル ポリシーの順序を変更するには、3 つのドット (その他の操作) を選択して、**[上へ移動]** または **[下へ移動]** を選択します。

ウィザードを完了すると、ラベル ポリシーが自動的に発行されます。

詳細については、「[秘密度ラベルとそのポリシーを作成して構成する](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)」を参照してください。