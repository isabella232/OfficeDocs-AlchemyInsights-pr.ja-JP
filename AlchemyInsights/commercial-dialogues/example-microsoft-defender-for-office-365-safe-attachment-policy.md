---
title: Microsoft Defender for Office 365 の安全な添付ファイル ポリシーの例
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751309"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Microsoft Defender for Office 365 の安全な添付ファイル ポリシーの例

これらの設定により、メッセージをすぐに配信し、スキャン後に添付ファイルを再添付する "*遅延なし*" というポリシーが有効になります。

- **名前**: 遅延なし
- **説明**: メッセージをすぐに配信し、スキャン後に添付ファイルを再添付します。
- **応答**: **[動的配信]** オプションを選択します。 詳細については、「[安全な添付ファイル ポリシー内の動的配信](https://go.microsoft.com/fwlink/?linkid=2092328)」を参照してください。
- **[添付ファイルをリダイレクト]** セクションで、**[リダイレクトを有効にする]** オプションを選択して、悪意のある添付ファイルを調査する Microsoft 365 のグローバル管理者、セキュリティ管理者、またはセキュリティ アナリストのメール アドレスを入力します。
- [**適用先**] セクションで、[**受信者のドメイン**] を選んでから、自分のドメインを選びます。 [**追加**] を選択し、[**OK**] を選択します。 完了したら、[**保存**] を選択します。

詳細については、「[Microsoft Defender for Office 365 のフィッシング詐欺対策ポリシーを構成する](https://go.microsoft.com/fwlink/?linkid=2092213)」を参照してください。
