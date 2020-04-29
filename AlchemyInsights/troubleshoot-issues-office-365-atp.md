---
title: Office 365 Advanced Threat Protection (ATP) に関する問題のトラブルシューティング
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766750"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Office 365 ATP の問題のトラブルシューティング

- **メール メッセージ配信の遅延通知する**? ATP の安全な添付ファイル ポリシーに動的配信オプションを使用してみてください。 これにより、受信者を悪意のあるファイルから保護しながら、メール メッセージの配信遅延を回避できます。
- **誤検知を報告しますか**? 分析用にファイルを送信するには、このリンクを使用してください: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **組織内のユーザーの間で送信されるメールに対して ATP 安全なリンクの保護を有効にできることをご存知ですか**? 次の手順を実行します。
    1. https://protection.office.comに移動して、サインインします。
    2. **脅威管理** > **ポリシー** > **安全なリンク**に移動します。
    3. **[特定の受信者に適用されるポリシー]** で、ポリシーを編集 (または追加) します。
    4. **組織内で送信されたメッセージに安全なリンクを適用する**を選択します。
    5. ポリシーを保存し、変更がデータセンターに反映されるまで約 30 分かかります。
- ATP の詳細については、「[Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)」を参照してください。