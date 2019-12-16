---
title: 2681 Office 365 の攻撃シミュレータ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2019
ms.locfileid: "37313941"
---
# <a name="attack-simulator-in-office-365"></a>Office 365 の攻撃シミュレータ

- 攻撃シミュレータが見つかりませんか ? 攻撃シミュレータには、**Office 365 Advanced Threat Protection プラン 2 (ATP プラン 2)** または **Office 365 Enterprise E5** が必要です。 攻撃シミュレータは、Office 365 Advanced Threat Protection プラン 1 (ATP プラン 1)、Office 365 Enterprise E3、または Office 365 Business サブスクリプションには含まれて**いません**。

- シミュレートされた攻撃を開始するために使用するアカウントには、グローバル管理者またはセキュリティ管理者のアクセス許可および多要素認証 (MFA) が必要です。 攻撃シミュレータの要件の詳細情報については、[このトピック](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)を参照してください。

- **ブルート フォース パスワード**攻撃シミュレーションに関する重要な注意事項:

  - ターゲット アカウントで MFA が有効になっており、パスワードが正しく推測された場合、アカウントは危険にさらされているものとして表示されません (2 番目の認証要素は不完全です)。

  - パスワード ファイルは 10 MB を超えることはできません。 1 行に 1 つのパスワードを使用し、リストの最後のパスワードの後に空白行 (キャリッジ リターン) を含めます。

- **スピア フィッシング**攻撃のシミュレーションに関する重要な注意事項:

  - 仕様上、**フィッシング ログイン サーバーの URL** にカスタム値を指定することはできません。

  - 受信者が[レポート メッセージ アドインを有効にする](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)を使用してメッセージをフィッシングとして報告する場合、メッセージのアラートを受信しない場合があります (シミュレートされた攻撃であるため)。

- レポート: シミュレートされた攻撃が完了したら、[**攻撃の詳細**] をクリックしてレポートを確認できます。

- 攻撃シミュレータの詳細な手順および新機能については、「[Office 365 の攻撃シミュレータ](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)」を参照してください。
