---
title: 2609 の保持または電子情報開示の保留
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/05/2019
ms.locfileid: "38006840"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>SharePoint Online または OneDrive for Business でアイテムを削除できない

ユーザーが SharePoint Online または OneDrive for Business のアイテムを削除できない場合があります。これは、アイテム保持ポリシー、保持ラベル、または電子情報開示の保留が OneDrive サイトの SharePoint サイトや特定のアイテムに適用されているためです。 この場合、ドキュメント、ドキュメントのバージョン、フォルダー、ドキュメント ライブラリ、リスト、アプリ、サイト、またはサイト コレクションを削除することはできません。 保持されているアイテムを削除しようとすると、次のエラーメッセージが表示されることがあります。

- "このサイトは、電子情報開示の保留またはアイテム保持ポリシーに含まれているため削除できません"
- "このサイトには、削除をブロックするコンプライアンス ポリシーが設定されています"
- "コンプライアンス ポリシーは現在このサイトの削除をブロックしています"
- "このサイト コレクションは、電子情報開示の保留またはアイテム保持ポリシーに含まれているサイトを含むため削除できません"
- "フォルダーを削除する前に、このフォルダー内のすべてのアイテムを削除する必要があります"
- "このアイテムのバージョンは保留中であるか、またはアイテム保持ポリシーにより、削除できません。
- "保留中のアイテムを削除することはできません"
- このアイテムに適用されるラベルにより、編集や削除ができません。
- "保留中またはアイテム保持ポリシーにより、リストを削除することはできません"
- "リストがブロックされている場合やアイテム保持ポリシーが適用されている場合は削除できません"

これらのシナリオでアイテムを削除するには、アイテム保持ポリシー、保持ラベル、または電子情報開示の保留を削除する必要があります (または、サイトをアイテム保持ポリシーから除外する必要があります)。 この問題の原因となっている保留を無効にするか除外する必要があります。 アイテム保持ポリシーまたは保留を削除すると、この変更が反映されるまでに最大で 24 時間かかる場合があります。 

SharePoint サイトや OneDrive アカウントに適用できるさまざまな保持機能と保留機能については、次のいずれかのトピックを参照してください。

- [アイテム保持ポリシーの概要](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [保持ラベルの概要](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Advanced eDiscovery の保留を管理する](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [電子情報開示の保留](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [従来のサイト クローズと削除のポリシー](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
