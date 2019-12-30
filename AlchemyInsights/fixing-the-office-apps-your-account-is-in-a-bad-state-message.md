---
title: Office アプリのアカウントの状態が正しくありません。エラーを修正する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886880"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Office アプリの "アカウントの状態が正しくありません。" エラーを修正する

このエラーを修正するには、影響を受けているコンピューター上で以下のオプションを試してみてください。

- Office アプリを開き、[**ファイル**] > [**アカウント**] > [**すべてのアカウントからサインアウト**] を選択します。 ライセンスが有効なユーザー アカウントを使用して、もう一度サインインします。 詳細については、「[Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。
- Windows 資格情報マネージャーを使用して、[Office の資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。<br>
  **注:** Office 2016 のレジストリ パスは 16.0 に変更されています。 たとえば、\Software\Microsoft\Office\16.0\Common\Identity\
- 影響を受けるコンピューター上で、次の手順に従い EnableADAL = 0 を設定します。  
     1. [Windows] ボタンを右クリックし、[**実行**] を選択します。 [**名前**] ボックスに **regedit** と入力し、[**OK**] を選択します。
     2. レジストリ エディターがデバイスに変更を加えられるようにするかどうかを尋ねるプロンプトが表示されたら、[**はい**] を選択します。
    3. レジストリ エディターで、HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity の下に EnableADAL の DWORD 値を 0 の設定で追加します。
- Office 2013 を使用して Office 365 に接続している最中にエラーが発生した場合には、Office クライアントの[モダンな認証を有効](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)にします。

詳細については、「[How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune (Office 365、Azure、または Intune にサインインできない非ブラウザー アプリのトラブルシューティング)](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)」を参照してください。

