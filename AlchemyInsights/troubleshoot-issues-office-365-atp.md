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
ms.openlocfilehash: d6170ac52b9af4d2bc6f8822ff2a9b8c1b161ed9
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544763"
---
# <a name="troubleshoot-issues-with-microsoft-defender-for-office-365"></a>Microsoft Defender for Office 365 の問題のトラブルシューティング

- **メール メッセージ配信を使用して遅延を通知しますか**? Microsoft Defender for Office 365 の安全な添付ファイル ポリシーの [動的配信] オプションをお試しください。 これにより、受信者を悪意のあるファイルから保護しながら、メール メッセージの配信遅延を回避できます。
- **誤検知を報告しますか**? [報告エクスプローラー](https://protection.office.com/reportsubmission)を使用しましょう。
- **組織内のユーザーの間で送信されるメールに対して Microsoft Defender for Office 365 安全なリンクの保護を有効にできることをご存知ですか**? 次の手順を実行します。
    1. https://protection.office.comに移動して、サインインします。
    2. **脅威管理** > **ポリシー** > **安全なリンク** に移動します。
    3. **[特定の受信者に適用されるポリシー]** で、ポリシーを編集 (または追加) します。
    4. **組織内で送信されたメッセージに安全なリンクを適用する** を選択します。
    5. ポリシーを保存し、変更が適用されるまでに最長で 30 分お待ちください。

- Microsoft Defender for Office 365 に関するその他のヘルプ情報を入手するには、「[Microsoft Defender for Office 365](/microsoft-365/security/office-365-security/office-365-atp)」を参照してください。