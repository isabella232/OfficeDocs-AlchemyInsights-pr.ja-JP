---
title: 2609-保持または電子情報開示の保留
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/05/2019
ms.locfileid: "38006840"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>SharePoint Online または OneDrive for Business のアイテムを削除できません

ユーザーが sharepoint Online または OneDrive for business のアイテムを削除できない場合があります。これは、アイテム保持ポリシー、保持ラベル、または電子情報開示の保留が OneDrive サイトの SharePoint または特定のアイテムに適用されるためです。 これには、ドキュメント、ドキュメントバージョン、フォルダー、ドキュメントライブラリ、リスト、アプリ、サイト、サイトコレクションを削除することはできません。 保持されているアイテムを削除しようとした場合に表示されるエラーメッセージの例を次に示します。

- "このサイトは、電子情報開示の保留またはアイテム保持ポリシーに含まれているため、削除できません"
- "このサイトには、削除をブロックするためのコンプライアンスポリシーが設定されています。
- "コンプライアンスポリシーは現在、このサイトの削除をブロックしています"
- "このサイトコレクションは、電子情報開示の保留またはアイテム保持ポリシーに含まれるサイトが含まれているため、削除できません。"
- "フォルダーを削除する前に、このフォルダー内のすべてのアイテムを削除する必要があります"
- "このアイテムのバージョンは、保留中またはアイテム保持ポリシーにあるため削除できません"
- "保留中にアイテムを削除することはできません"
- "このアイテムに適用されているラベルは、編集または削除されないようにします。
- "保留中またはアイテム保持ポリシーでリストを削除できません"
- "リストは、ブロックされている場合、またはアイテム保持ポリシーが適用されている場合は削除できません"

これらのいずれかのシナリオでアイテムを削除するには、アイテム保持ポリシー、保持ラベル、または電子情報開示ホールドを削除する必要があります (または、サイトをアイテム保持ポリシーから除外する必要があります)。 この問題の原因となっている各保留リストを無効にするか、または除外する必要があります。 アイテム保持ポリシーまたはホールドを削除した後は、変更が反映されるまでに最大24時間かかる場合があります。 

SharePoint サイトと OneDrive アカウントに適用できるさまざまな保持および保持機能の詳細については、以下のいずれかのトピックを参照してください。

- [アイテム保持ポリシーの概要](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [保持ラベルの概要](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [詳細な電子情報開示で保留リストを管理する](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [電子情報開示の保持](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [従来のサイトの閉鎖および削除ポリシー](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
