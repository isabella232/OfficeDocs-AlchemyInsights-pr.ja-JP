---
title: Microsoft Defender for Office365 の一般的な問題を修正する
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330065"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Microsoft Defender for Office365 の一般的な問題を修正する

Microsoft Defender for Office365 の一般的な問題に対するいくつかの解決策を次に示します。

- **メッセージの遅延**:

  メール配信の遅延は、メッセージの添付ファイルセーフによって発生する可能性があります。 詳細については、「添付ファイルポリシー[設定セーフを参照してください](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)。

- **誤検知または負の結果を報告する**:

  詳細については、「[メッセージとファイルを Microsoft に報告する](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)」を参照してください。

- **[リンクセーフを有効にする**:

  1. [ポリシー] Microsoft 365 Defenderで、[ポリシー] セクション&の [&脅威ポリシーとリンクセーフメールを送信する] <https://security.microsoft.com/>  \>  \>  \> **に移動** します。

     [リンク] ページに直接 **移動セーフを** 使用します <https://security.microsoft.com/safelinksv2> 。

  2. [リンク **セーフ] ページ** で、ポリシーの名前をクリックしてポリシーを選択します。
  3. 表示される詳細フライアウトで、次のいずれかの手順を実行します。
     - 新しいポリシーを作成するには、**[+ 作成]** を選択します。 ポリシー設定の定義に役立つウィザードが起動します。
     - 既存のポリシーを編集するには、ポリシーの名前をクリックしてポリシーを選択します。 表示される詳細フライアウトで、[保護の設定]**セクションで [編集****] を選択** します。
  4. [保護の **設定] ページ** で、次の設定を構成します。
     - [メッセージ内の不明な潜在的に悪意のある URL の **アクションを選択する] をオンにします**。
     - **組織内で送信されたメッセージに安全なリンクを適用する** を選択します。

  詳細については、「Microsoft Defender for セーフのリンク ポリシーをセットアップする[」を参照Office 365。](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
