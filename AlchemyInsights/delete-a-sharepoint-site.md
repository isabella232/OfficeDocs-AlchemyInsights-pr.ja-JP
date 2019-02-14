---
title: SharePoint サイトを削除する
ms.author: kirks
author: Techwriter40
ms.date: 1/24/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c060815d-1d3f-4a13-81c2-0377bbeda202
ms.openlocfilehash: f6ee16a20f2280ba4d8d28ab3fdb4672cd9963b5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927581"
---
# <a name="delete-a-sharepoint-site"></a>SharePoint サイトを削除する
 **新しい SharePoint 管理センターからサイトを削除する**
  
アクティブなサイトを削除するには、現在の SharePoint 管理センターに移動して、右上で [今すぐ使ってみる] をクリックします。[**アクティブなサイト**] を選択してそのサイトを選び、[**削除**] を選択します。[新しい SharePoint 管理センターで削除されたサイトを表示または復元する](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)には、[**削除されたサイト**] を選択します。詳細については、「[新しい SharePoint 管理センターのサイトを管理する](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center)」を参照してください。
  
**重要:** サイトがアイテム保持ポリシーの一部である場合は、[セキュリティ&amp;コンプライアンス管理センター](https://protection.office.com/?rfr=AdminCenter#/homepage)からそのサイトが削除されるまで、サイトを削除できない場合があります。詳細については、「[アイテム保持ポリシーの概要](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites)」を参照してください。 
  
ヒント:
- グローバル管理者と SharePoint 管理者は、**Office 365 グループ**に属しているサイトを削除できるようになりました。これにより、グループとそのグループのすべてのリソース (Outlook メールボックス、予定表、Teams チャンネルなど) が削除されます。詳細については、[SharePoint サイトの削除](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)に関するページを参照してください。
- 削除されたサイトは 93 日間復元できます。削除されたグループは 30 日以内に復元する必要があります。詳細については、[削除されたサイトの表示と復元](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)に関するページを参照してください。
- PowerShell を使ってサイトを完全に削除するには、[Remove-SPSite](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps) コマンドレットの例を参照してください。 
  

