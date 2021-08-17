---
title: SharePoint サイトを作成する
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080895"
---
# <a name="create-a-sharepoint-site"></a>SharePoint サイトを作成する

SharePoint 管理センターで[アクティブなサイト](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true)からサイトを作成または管理します。 詳細については、「[新しい SharePoint 管理センターでサイトを管理する](https://docs.microsoft.com/sharepoint/manage-site-creation)」を参照してください。 

## <a name="tips"></a>ヒント:

- 既存のサイトと同じ URL を持つサイトを作成することは **できません**。サイトを削除し、その URL を再利用する場合は、削除したサイトが [[削除されたサイト]](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) 下にまだ存在する可能性があります。URL を再利用するには、サイトを完全に削除する必要があります。Powershell を使用してサイトを完全に削除するには、[Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) コマンドレットの例を参照してください。
- ユーザーによっては、サイトを作成できない場合があります。[「SharePoint Online のサイト作成を管理する」を参照してください](https://docs.microsoft.com/sharepoint/manage-site-creation)。
- サイトが **作成中に** 予想より長く停止しているように見えることがあります。この問題が初めて発生してから 24 時間以上経過している場合は、サポート チケットを記録してください。多くの場合は、Microsoft が既に解決策に取り組んでいます。解決策の完成までには 24 時間以上の時間がかかります。
