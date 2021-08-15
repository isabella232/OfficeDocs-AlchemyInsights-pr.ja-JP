---
title: Domain Services の構成
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: cf8ea7d73adf36f71ae92abad48ef9b664eb0c96094a38750c86cf42958b5323
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994762"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>AAD-DS を有効にできないか、展開に失敗する

Azure AD Domain Services (AAD-DS) が有効になっていない、または展開できない問題を解決するには、次の手順を実行します。

1. 既存の仮想ネットワークを使用している場合は、ポータル https://aka.ms/aadds-networking の AAD-DS で同期するために必要なポートをブロックする規則がないか NSG を確認します。
2. エラー メッセージが、https://aka.ms/aadds-troubleshoot-enable で利用可能なこのトラブルシューティング ガイドに記載されているかどうかを確認します。
3. 新しい仮想ネットワークに Azure AD Domain Services を展開してみます。
4. AAD-DS の展開方法については、「[AAD Domain Services の作成と構成](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)」で作業の開始ガイドに従います。
5. Azure AD Domain Services の展開に問題がある場合は、「[Azure AD Domain Services のトラブルシューティング](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)」を参照して、作業を再開するための一般的なエラーを解決してください。 

**AAD-DS を無効にできない**

AD-DS を一時停止できません。 管理対象ドメインの使用を停止する場合は、ドメインを削除する必要があります。
管理対象ドメインを削除するには、「[AAD Domain Services の削除](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)」を参照してください。



