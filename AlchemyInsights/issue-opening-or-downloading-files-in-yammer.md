---
title: Yammer でファイルを開いたり、ダウンロードしたりする際の問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028261"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Yammer でファイルを開いたり、ダウンロードしたりする際の問題

従来の Yammer は、メッセージおよびグループへのファイルのアップロードについて、複数のオプションをサポートしています。 ネットワーク構成によっては、ファイルは、既定で SharePoint のストレージに保存されます。

新しい Yammer のファイルピッカーは、従来の Yammer で使用可能なすべてのオプションをまだサポートしていません。 今後の更新で、追加の機能が追加されます。 詳しくは、[「Yammer の会話の投稿にファイルまたは画像を添付する」](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)をご覧ください。

**ファイルを開くことができない、またはダウンロードすることができない**  

ファイルを Yammer にアップロードしたり、SharePoint Online のファイルにリンクしたりすることもできます。 トラブルシューティングを行うには、まずファイルの場所を特定する必要があります。 ファイルが Yammer にアップロードされている場合、ファイルの URL は * yammer.com です。 必要な URLと IP アドレスがブロック解除されていることを確認します。 詳細については、ブログの投稿[Yammer にハードコードされた IP アドレスを使用することはお勧めできません](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)を参照してください。

グローバル管理者でもあるユーザーがファイルをダウンロードできるかどうかを確認します。 ファイルが個人用の場合、プライベートコンテンツモードを使用する必要がある可能性があります。 詳細については、[「Yammerでプライベートコンテンツ を監視する」](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)を参照してください。  

**Yammer ネットワークのゲストと SharePoint Online のファイル**  

[Yammer のネットワークゲスト](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests)は、Azure AD B2B を使わず、Yammer サービスの内部にあるため、SharePoint に保存されている Yammer ファイルにアクセスできません。 ID を使用して、SharePoint Online のドキュメントライブラリにアクセスできる外部 AAD B2B ユーザーを作成します。 Yammer での Azure AD B2B ゲストサポートの詳細については、[「Yammerプレビューで企業間 (B2B)での ゲストサポート- お客様のご利用規約と よくあるご質問」](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)を参照してください。