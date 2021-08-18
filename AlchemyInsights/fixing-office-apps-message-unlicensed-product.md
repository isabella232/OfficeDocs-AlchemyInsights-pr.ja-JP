---
title: Office をライセンス認証することができない
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327851"
---
# <a name="unable-to-activate-office"></a>Office をライセンス認証することができない

**注**: 以前のバージョンの Windows (Windows 7 など) を使用している場合は、TLS 1.2 が既定で有効になっていることを確認します。 詳細については、「[Windows の WinHTTP で TLS 1.1 および TLS 1.2 を既定のセキュリティ で保護されたプロトコルとして有効にするための更新プログラム](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)」を参照してください。

- サブスクリプションが期限切れの状態であるかどうかを確認します。
- Office 365 Business や Business Premium など、クライアント ライセンスが許可されているサブスクリプションを持っていること、そして[ユーザーにライセンスが割り当てられていることを確認](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)します。
- ユーザーが、ライセンスが割り当てられているアカウントと同じアカウントで Office にサインインしていることを確認します。
- [Office 365 サービス正常性ページ](https://docs.microsoft.com/office365/enterprise/view-service-health)を確認し、サービスに既知の問題があるかどうかを確認します。
- ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、Microsoft 365 アプリのインターネットへのアクセスをブロックしていないことを確認します。「[Office 365 URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL および IP アドレス範囲")」を参照してください。

**ヒント** Windows マシンでは、一般的な Office のサインインに関する問題のいくつかを診断し、自動的に修正することができます。 **[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA-OfficeSignInScenario)** をダウンロードして実行し、自動化ツールを使用します。

トラブルシューティングのための次の操作をお試しください。

- Office アプリを開き、すべての既存のユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。 Office のライセンスを[削除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)して[再び割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)、影響を受けているユーザー アカウントを使用して [Office にサインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)します。
- [ライセンス認証のトラブルシューティング ツール](https://aka.ms/SARA-OfficeActivation-Alchemy)を実行します。
- [Office のライセンス認証の状態を再設定します](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office のライセンス認証の状態をリセットする")。
- [Office のオンライン修復を実行します](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)。

その他のトラブルシューティングの手順については、次を参照してください。  

- [Office でのライセンスのない製品というエラーとライセンス認証のエラー](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Office のライセンス認証時の "申し訳ございません。お使いのアカウントに接続できません。後でもう一度やり直してください。" というエラー](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)