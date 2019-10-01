---
title: Office 365 の2681アタックシミュレータ
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2019
ms.locfileid: "37313941"
---
# <a name="attack-simulator-in-office-365"></a>Office 365 の攻撃シミュレータ

- アタックシミュレータはありませんか? アタックシミュレータには、 **office 365 Advanced Threat Protection プラン 2 (ATP Plan 2)** または**Office 365 Enterprise E5**が必要です。 アタックシミュレータは、Office 365 Advanced Threat Protection プラン 1 (ATP プラン 1)、Office 365 Enterprise E3、または任意の Office 365 Business サブスクリプションに含まれて**いません**。

- シミュレートされた攻撃を開始するために使用するアカウントには、グローバル管理者またはセキュリティ管理者のアクセス許可と多要素認証 (MFA) が必要です。 アタックシミュレータの要件の詳細については、[このトピック](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)を参照してください。

- **ブルートフォースパスワード**攻撃のシミュレーションに関して知っておくべき重要な点は次のとおりです。

  - ターゲットアカウントの MFA が有効になっており、パスワードが正しく推測されている場合、そのアカウントは侵害されたとして表示されません (2 番目の認証要素は不完全になります)。

  - パスワードファイルは、10 MB を超えることはできません。 行ごとに1つのパスワードを使用し、リスト内の最後のパスワードの後に空白行 (復帰) を含めます。

- **スピアーフィッシング**接続のシミュレーションに関して知っておくべき重要な点は次のとおりです。

  - 設計上、**フィッシングのログインサーバーの URL**にカスタム値を指定することはできません。

  - 受信者が [[レポートメッセージを有効](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)にする] アドインを使用してメッセージをフィッシングとして報告する場合、メッセージの通知を受信しないことがあります (これはシミュレートされた攻撃です)。

- レポート: シミュレートされた攻撃が完了したら、[**アタックの詳細**] をクリックしてレポートを表示できます。

- アタックシミュレータの詳細な手順と新機能については、「 [Office 365 のアタックシミュレータ](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)」を参照してください。
