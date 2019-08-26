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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051953"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Office アプリでの「申し訳ございません。このコンピューターに、組織内の別のアカウントが既にサインインしています」というメッセージを解決する

このエラーを解決するには、次の操作を行います。

- 影響を受けているアカウント以外のすべての職場のアカウントを削除します。これを行うには、[Windows の設定] > [**職場または学校にアクセスする**] に移動します。
- Windows 資格情報マネージャーを使用して、[Office の資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。<br/>
    **注:** Office 2016 のレジストリ パスは 16.0 に変更されています。 (例: \Software\Microsoft\Office\16.0\Common\Identity\)
- Office アプリを開き、[**ファイル**]  >  [**アカウント**]  >  [**サインアウト**] を選択します。その後、有効なライセンスがあるユーザー アカウントでサインインします。 詳細については、「[Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。
- Mac の場合は、「[Office 2016 for Mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください。

詳細については、Office での「[申し訳ございません。このコンピューターに、組織内の別のアカウントが既にサインインしています](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)」を参照してください。