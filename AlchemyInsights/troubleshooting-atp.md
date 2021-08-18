---
title: Microsoft Defender for Office 365 のトラブルシューティング
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 5614deae44c08b2a5f9786b26bdbdcfa4daed15d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330821"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Microsoft Defender for Office 365 のトラブルシューティング

- **メッセージの配信に遅延がある場合** Microsoft Defender for Office 365 の安全な添付ファイル ポリシーの [[動的配信]](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) オプションを使用します。 これにより、メッセージの遅延を回避すると同時に、悪意のあるファイルから受信者を保護できるようになります。

- **Microsoft に誤検知を報告するには**、[報告エクスプローラー](https://protection.office.com/reportsubmission)を使用します。

-** 組織内の受信者間で送信される内部メールに安全なリンクの保護機能を有効にする方法をご存知ですか? 手順は次のとおりです。

  1. [https://protection.office.com](https://protection.office.com) に移動して、全体管理者またはセキュリティ管理者のアカウントでサインインします。

  2. 左側のナビゲーション ウィンドウにある **[脅威の管理]** で、**[ポリシー]** \> **[安全なリンク]** を選択します。

  3. **[組織全体に適用されるポリシー]** セクションで、ポリシーを選択して **[編集]** をクリックします。

  4. **[設定]** の下側にある **[組織内で送信されるメッセージに安全なリンクを適用する]** を有効にします。
