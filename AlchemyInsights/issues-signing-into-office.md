---
title: Office アプリへのサインインの問題
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051954"
---
# <a name="issues-signing-in-to-office-apps"></a>Office アプリへのサインインの問題

Office アプリのサインインの問題を修正するには、次の操作を行います。

- Windows の設定を使用して、影響を受けるアカウントを除くすべてのワークアカウントを削除します。 >**職場または学校にアクセス**します。
- Windows 資格情報マネージャーを使用して[Office 資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。<br/>
    **注:** Office 2016 のレジストリパスは16.0 に変更されました。 (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Office アプリを開き、[**ファイル** > **アカウント** > の**サインアウト**] を選択します。次に、有効なライセンスを持つユーザーアカウントを使用してサインインします。 詳細については、「 [Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。
- Mac の場合は、「 [Office 2016 For mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください。
- Office 2013 を使用して Office 365 に接続しているときにエラーが発生する場合は、Office クライアントの先進認証を有効にします。

詳細については、以下を参照してください。
- [Office 365、Azure、または Intune にサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Windows 10 の Office 2016 ビルド16.0.7967 に更新後のサインインにおける接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [「申し訳ございません。組織からの別のアカウントは、このコンピューターに既にサインインしています」という Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [ADFS を使用する場合の Office モダン認証に関するサインインの問題のトラブルシューティング](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)