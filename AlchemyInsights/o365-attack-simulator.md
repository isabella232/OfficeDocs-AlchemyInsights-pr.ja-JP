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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545731"
---
# <a name="attack-simulator-in-microsoft-365"></a>Microsoft 365 の攻撃シミュレータ

- 攻撃シミュレータが見つかりませんか ? 攻撃シミュレータには、**Microsoft Defender for Office 365 プラン 2** または **Office 365 Enterprise E5** が必要です。 攻撃シミュレータは、Microsoft Defender for Office 365 プラン 1、Office 365 Enterprise E3、または Microsoft 365 Apps for business サブスクリプションには含まれて **いません**。

- シミュレートされた攻撃を開始するために使用するアカウントには、グローバル管理者またはセキュリティ管理者のアクセス許可および多要素認証 (MFA) が必要です。 攻撃シミュレータの要件の詳細情報については、[このトピック](/microsoft-365/security/office-365-security/attack-simulator)を参照してください。

- **ブルート フォース パスワード** 攻撃シミュレーションに関する重要な注意事項:

  - ターゲット アカウントで MFA が有効になっており、パスワードが正しく推測された場合、アカウントは危険にさらされているものとして表示されません (2 番目の認証要素は不完全です)。

  - パスワード ファイルは 10 MB を超えることはできません。 1 行に 1 つのパスワードを使用し、リストの最後のパスワードの後に空白行 (キャリッジ リターン) を含めます。

- **スピア フィッシング** 攻撃のシミュレーションに関する重要な注意事項:

  - 仕様上、**フィッシング ログイン サーバーの URL** にカスタム値を指定することはできません。

  - 受信者が[レポート メッセージ アドインを有効にする](/microsoft-365/security/office-365-security/enable-the-report-message-add-in)を使用してメッセージをフィッシングとして報告する場合、メッセージのアラートを受信しない場合があります (シミュレートされた攻撃であるため)。

- レポート: シミュレートされた攻撃が完了したら、[**攻撃の詳細**] をクリックしてレポートを確認できます。

- 攻撃シミュレータの詳細な手順および新機能については、「[Microsoft 365 の攻撃シミュレータ](/microsoft-365/security/office-365-security/attack-simulator)」を参照してください。
