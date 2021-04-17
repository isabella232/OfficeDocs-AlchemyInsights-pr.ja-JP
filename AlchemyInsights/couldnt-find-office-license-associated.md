---
title: Microsoft 365 アプリの「関連する Office ライセンスが見つかりませんでした」メッセージの修正
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816493"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Microsoft 365 アプリの「関連する Office ライセンスが見つかりませんでした」メッセージの修正

このメッセージが表示された場合は、次を試してください。

1. ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Microsoft 365 アプリにアクセスするのをそれらがブロックしていないことを確認します。 「[Microsoft 365 の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。
2. Office ライセンスを削除し、影響を受ける[ユーザーに再割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)します。 
3. Office アプリを開き、既存のすべてのユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。
4. Windows の設定、[**アカウント**] > [**メールとアカウント**] の順に移動し、影響を受けるアカウントを除くすべての職場アカウントを削除します。
5. Windows の設定、[**アカウント**] > [**職場または学校にアクセスする**] の順に移動し、影響を受けるアカウントを除くすべての職場アカウントを切断します。
6. Office のライセンス認証の状態をリセットします。 [詳細情報](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)を参照してください。
7. 影響を受けるアカウントを使用して[サインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) します。

その他のトラブルシューティング ソリューションについては、「[Office でのライセンスのない製品エラーとアクティブ化エラー](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)」に関するページを参照してください。