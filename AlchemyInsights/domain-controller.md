---
title: 'ドメイン コントローラ '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901720"
---
# <a name="domain-controller"></a>ドメイン コントローラ

**AAD-DS を有効にできないか、展開が失敗しています**

Azure AD Domain Services (AAD-DS) が有効になっていない、または展開できない問題を解決するには、次の手順を実行します。

1. 既存の仮想ネットワークを使用している場合は、ポータル https://aka.ms/aadds-networking の AAD-DS で同期するために必要なポートをブロックする規則がないか NSG を確認します。
2. エラー メッセージが、https://aka.ms/aadds-troubleshoot-enable で利用可能なこのトラブルシューティング ガイドに記載されているかどうかを確認します。
3. 新しい仮想ネットワークに Azure AD Domain Services を展開してみます。
4. [Azure AD ドメイン サービスを作成するためのチュートリアル](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)で利用できる AAD-DS の展開方法については、「作業の開始ガイド」に従ってください。
5. Azure AD Domain Services の展開に問題がある場合は、「[Azure AD Domain Services のトラブルシューティング](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)」を参照して、作業を再開するための一般的なエラーを解決してください。 

**AAD-DS を無効にできない**

AD-DS を一時停止できません。 管理対象ドメインの使用を停止する場合は、ドメインを削除する必要があります。

問題が発生した場合、一般的なエラー メッセージを解決するため、および関連するトラブルシューティングの手順については、「[Azure ActiveDirectoryドメインサービスのトラブルシューティング](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)」を参照してください。
