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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051953"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Office アプリを修正する "申し訳ありません。組織からの別のアカウントは既にサインインしています" というメッセージが表示される

このエラーを解決するには、次の操作を行います。

- Windows の設定を使用して、影響を受けるアカウントを除くすべてのワークアカウントを削除します。 >**職場または学校にアクセス**します。
- Windows 資格情報マネージャーを使用して[Office 資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。<br/>
    **注:** Office 2016 のレジストリパスは16.0 に変更されました。 (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Office アプリを開き、[**ファイル** > **アカウント** > の**サインアウト**] を選択します。次に、有効なライセンスを持つユーザーアカウントを使用してサインインします。 詳細については、「 [Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。
- Mac の場合は、「 [Office 2016 For mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください。

詳細については、「 [Office の組織からの別のアカウントが既にこのコンピューターにサインイン](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)しています。」を参照してください。