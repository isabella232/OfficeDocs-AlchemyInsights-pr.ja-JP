---
title: Office アプリへのサインインに関する問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051954"
---
# <a name="issues-signing-in-to-office-apps"></a>Office アプリへのサインインに関する問題

Officeアプリでのサインインの問題を修正するには、次の操作を試してください。

- 影響を受けているアカウント以外のすべての職場のアカウントを削除します。これを行うには、[Windows の設定] > [**職場または学校にアクセスする**] に移動します。
- Windows 資格情報マネージャーを使用して、[Office の資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。<br/>
    **注:** Office 2016 のレジストリ パスは 16.0 に変更されています。 (例: \Software\Microsoft\Office\16.0\Common\Identity\)
- Office アプリを開き、[**ファイル**]  >  [**アカウント**]  >  [**サインアウト**] を選択します。その後、有効なライセンスがあるユーザー アカウントでサインインします。 詳細については、「[Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。
- Mac の場合は、「[Office 2016 for Mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください。
- Office 2013 を使用し Office 365 へと接続する際にエラーが発生した場合、Office クライアントの先進認証を有効にします。

詳細については、次のトピックを参照してください。
- 「[Office 365、Azure、または Intune にサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)」
- 「[Windows 10 の Office 2016 ビルド16.0.7967 に更新後のサインインにおける接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」
- 「[Office での "申し訳ございません。このコンピューターに、組織内の別のアカウントが既にサインインしています"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)」
- 「[ADFS を使用している場合の Office 先進認証によるサインイン問題のトラブルシューティング](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)」