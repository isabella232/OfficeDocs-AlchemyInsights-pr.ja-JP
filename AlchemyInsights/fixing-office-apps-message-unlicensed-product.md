---
title: Office をライセンス認証することができない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704935"
---
# <a name="unable-to-activate-office"></a>Office をライセンス認証することができない

- サブスクリプションが期限切れの状態であるかどうかを確認します。
- Office 365 Business や Business Premium など、クライアント ライセンスが許可されているサブスクリプションを持っていること、そして[ユーザーにライセンスが割り当てられていることを確認](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)します。
- ユーザーが、ライセンスが割り当てられているアカウントと同じアカウントで Office にサインインしていることを確認します。
- [Office 365 サービス正常性ページ](https://docs.microsoft.com/office365/enterprise/view-service-health)を確認し、サービスに既知の問題があるかどうかを確認します。
- ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、Microsoft 365 アプリがインターネットにアクセスするのをそれらがブロックしていないことを確認します。 詳細については、「[Office 365 の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL および IP アドレス範囲")」を参照してください。

Windows コンピューターについての **ヒント**、Office の一般的なサインインの問題を診断して、自動的に修正することができます。 **[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA-OfficeSignInScenario)** をダウンロードして実行し、自動化ツールを使用します。

トラブルシューティングのための次の操作をお試しください。

- Office アプリを開き、すべての既存のユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。 Office のライセンスを[削除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)して[再び割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)、影響を受けているユーザー アカウントを使用して [Office にサインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)します。
- [ライセンス認証のトラブルシューティング ツール](https://aka.ms/SARA-OfficeActivation-Alchemy)を実行します。
- [Office のライセンス認証の状態を再設定します](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office のライセンス認証の状態をリセットする")。
- [Office のオンライン修復を実行します](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)。

その他のトラブルシューティングの手順については、次を参照してください。  

- [Office でのライセンスのない製品というエラーとライセンス認証のエラー](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Office のライセンス認証時の "申し訳ございません。お使いのアカウントに接続できません。後でもう一度やり直してください。" というエラー](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)