---
title: ライセンスのない製品というエラーを解決する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 89d0e589329d40f17c36baa54868154be0f5b887
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582744"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>"ライセンスのない製品" エラーの解決方法の提案

"ライセンスのない製品" エラーを解決するには、次の操作を行います。

- サブスクリプション ステータスが期限切れになっていないかどうか確認します。
- Microsoft 365 Apps for business や Business Premium など、クライアント ライセンスが許可されているサブスクリプションを持っていること、[ユーザーにライセンスが割り当てられていることを確認します](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。 
- ユーザーが、ライセンスが割り当てられているアカウントと同じアカウントで Office にサインインしていることを確認します。
- [サービス正常性ページ](https://docs.microsoft.com/office365/enterprise/view-service-health)を確認し、サービスに既知の問題があるかどうかを確認します。
- ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、Microsoft 365 アプリがインターネットにアクセスするのをそれらがブロックしていないことを確認します。 「 [URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。

また、トラブルシューティングのための次の操作を試すこともできます。 

- Office アプリを開き、既存のすべてのユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。 Office のライセンスを[削除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)して[再び割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)、影響を受けているユーザー アカウントを使用して [Office にサインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)します。
- [ライセンス認証のトラブルシューティング ツール](https://aka.ms/SARA-OfficeActivation-Alchemy)を実行します。
- [Office のライセンス認証の状態をリセットします](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)。 
- [Office のオンライン修復を実行します](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)。

その他のトラブルシューティングの手順については、次を参照してください。 

- [Office でのライセンスのない製品というエラーとライセンス認証のエラー](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Office のライセンス認証時の "申し訳ございません。お使いのアカウントに接続できません。後でもう一度やり直してください。" というエラー](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)