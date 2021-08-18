---
title: Microsoft Defender for Office 365 の問題のトラブルシューティング
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 026e9722ac533e69178c40dd26792a362cf8fdda
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317191"
---
# <a name="troubleshoot-issues-with-microsoft-defender-for-office-365"></a>Microsoft Defender for Office 365 の問題のトラブルシューティング

- **メール メッセージ配信の遅延に気づいた場合は**、 Microsoft Defender for Office 365 の安全な添付ファイル ポリシーの [動的配信] オプションを使用してみてください。 これにより、受信者を悪意のあるファイルから保護しながら、メール メッセージの配信の遅延を回避できます。
- **誤検知を報告するには**、[報告エクスプローラー](https://protection.office.com/reportsubmission)を使用します。
- **組織内のユーザー間で送信されるメールに対して、Microsoft Defender for Office 365 の安全なリンクの保護を有効にするには**、次の手順を実行します。
    1. https://protection.office.comに移動して、サインインします。
    2. **脅威管理** > **ポリシー** > **安全なリンク** に移動します。
    3. **[特定の受信者に適用されるポリシー]** で、ポリシーを編集 (または追加) します。
    4. **組織内で送信されたメッセージに安全なリンクを適用する** を選択します。
    5. ポリシーを保存します。変更が適用されるまでに最長で 30 分かかる場合があります。

- Microsoft Defender for Office 365 に関するその他のヘルプ情報を入手するには、「[Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)」を参照してください。