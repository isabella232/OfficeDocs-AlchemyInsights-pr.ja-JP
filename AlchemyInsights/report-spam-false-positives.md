---
title: 迷惑メールの誤検知を Microsoft に報告しますか?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396620"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>正当なメッセージが迷惑メールとしてマークされていますか?

正当なメールが [迷惑メールに分類する] フォルダーまたは [検疫] に入ると、ストレスが発生します。 誤検知の最も一般的な理由を次に示します。

**テナントの上書き (最も一般的)** これは、完全なコントロールの下で修復できます。

影響を与えるポリシーとルールを分析するために、Microsoft 365 Defender にてメッセージを送信します。再スキャンの詳細は数分以内に確認できます。
必要に応じて、ポリシーまたはルールを確認または変更します。 

**エンドユーザーの上書き (最も一般的)** これは、完全なコントロールの下で修復できます。 

影響を与えるポリシーとルールを分析するために、Microsoft 365 Defender にてメッセージを送信します。再スキャンの詳細は数分以内に確認できます。 

メッセージがユーザーの受信拒否リストのアドレスから送信されたためにブロックされた場合、ヘッダーにはスパム対策フィルターの判定 "SFV:BLK" が含まれます。

**差出人のメール認証** これは、部分的なコントロールの下で修復できます。

メッセージを送信すると、送信時の差出人のメール認証のエラーを分析します。結果は 1 日以内に確認できます。 

送信側インフラストラクチャを所有している場合は、SPF、DKIM、DMARC と連携して、宛先のメール システムがドメインから送信されたメッセージを信頼していることを確認します。 または、差出人に連絡して DNS 構成に対応します。

**Microsoft のフィルターの判定** これは、部分的なコントロールの下で修復できます。

メッセージを送信し、メッセージが安全であることを報告します。再スキャンの結果は 1 日以内に確認できます。 特定の状況でフィルターの判定をすることに同意しない場合は、テナントの許可/禁止リストを使用します。 ただし、Microsoft のフィルターの判定を完全にバイパスしないでください。 

詳細については、以下を参照してください。

- エンド ユーザーが Microsoft にメッセージを送信できるようにします。 Microsoft は、提出された内容に基づき、メールの保護テクノロジの有効性を向上させます。また、提出された内容は、ポリシーの更新の指標として使用できるように提出レポートに表示されます。 

- 分析用のメッセージの送信に関する短いビデオを見るには、「[分析用のメッセージの送信](https://go.microsoft.com/fwlink/?linkid=2166435)」をご覧ください。

- [管理者送信を使用して、疑いがあるスパム、フィッシング、URL、ファイルを Microsoft に提出する](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [テナントの許可/禁止リストを管理する](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Microsoft 365 のスパム対策メッセージ ヘッダー](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [EOP の送信スパム保護](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)