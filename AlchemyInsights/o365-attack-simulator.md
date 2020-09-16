---
title: 2681 Microsoft 365 の攻撃シミュレータ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759224"
---
# <a name="attack-simulator-in-microsoft-365"></a>Microsoft 365 の攻撃シミュレータ

- 攻撃シミュレータが見つかりませんか ? 攻撃シミュレータには、**Office 365 Advanced Threat Protection プラン 2 (ATP プラン 2)** または **Office 365 Enterprise E5** が必要です。 攻撃シミュレータは、Office 365 Advanced Threat Protection プラン 1 (ATP プラン 1)、Office 365 Enterprise E3、または 一般法人向け Microsoft 365 アプリ サブスクリプションには含まれて**いません**。

- シミュレートされた攻撃を開始するために使用するアカウントには、グローバル管理者またはセキュリティ管理者のアクセス許可および多要素認証 (MFA) が必要です。 攻撃シミュレータの要件の詳細情報については、[このトピック](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)を参照してください。

- **ブルート フォース パスワード**攻撃シミュレーションに関する重要な注意事項:

  - ターゲット アカウントで MFA が有効になっており、パスワードが正しく推測された場合、アカウントは危険にさらされているものとして表示されません (2 番目の認証要素は不完全です)。

  - パスワード ファイルは 10 MB を超えることはできません。 1 行に 1 つのパスワードを使用し、リストの最後のパスワードの後に空白行 (キャリッジ リターン) を含めます。

- **スピア フィッシング**攻撃のシミュレーションに関する重要な注意事項:

  - 仕様上、**フィッシング ログイン サーバーの URL** にカスタム値を指定することはできません。

  - 受信者が[レポート メッセージ アドインを有効にする](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)を使用してメッセージをフィッシングとして報告する場合、メッセージのアラートを受信しない場合があります (シミュレートされた攻撃であるため)。

- レポート: シミュレートされた攻撃が完了したら、[**攻撃の詳細**] をクリックしてレポートを確認できます。

- 攻撃シミュレータの詳細な手順および新機能については、「[Microsoft 365 の攻撃シミュレータ](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)」を参照してください。
