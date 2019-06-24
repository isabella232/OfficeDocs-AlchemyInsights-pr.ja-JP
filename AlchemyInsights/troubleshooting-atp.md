---
title: Office 365 Advanced Threat Protection のトラブルシューティング
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: b4358fb55a1145833510c6063b520d822f2d1eaf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35085891"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a>Office 365 Advanced Threat Protection のトラブルシューティング

- メッセージの配信に遅延がある場合 ATP の安全な添付ファイル ポリシーの [[動的配信]](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) オプションを使用します。 これにより、メッセージの遅延を回避すると同時に、悪意のあるファイルから受信者を保護できるようになります。

- Microsoft に誤検知を報告する場合 この[リンク](https://www.microsoft.com/wdsi/filesubmission/)を使用して、分析用にファイルを送信してください。

- 組織内の受信者間で送信される内部電子メールに安全なリンクの保護機能を有効にする方法 次の手順を実行します。

  1. [https://protection.office.com](https://protection.office.com) に移動して、全体管理者またはセキュリティ管理者のアカウントでサインインします。

  2. 左側のナビゲーション ウィンドウにある **[脅威の管理]** で、**[ポリシー]** \> **[安全なリンク]** を選択します。

  3. **[組織全体に適用されるポリシー]** セクションで、ポリシーを選択して **[編集]** をクリックします。

  4. **[設定]** の下側にある **[組織内で送信されるメッセージに安全なリンクを適用する]** を有効にします。
