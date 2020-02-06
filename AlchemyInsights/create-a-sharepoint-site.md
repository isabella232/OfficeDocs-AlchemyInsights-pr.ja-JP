---
title: SharePoint サイトを作成する
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770860"
---
# <a name="create-a-sharepoint-site"></a>SharePoint サイトを作成する

SharePoint 管理センターで[アクティブなサイト](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true)からサイトを作成または管理します。 詳細については、「[新しい SharePoint 管理センターでサイトを管理する](https://docs.microsoft.com/sharepoint/manage-site-creation)」を参照してください。 

## <a name="tips"></a>ヒント:

- 既存のサイトと同じ URL のサイトを作成することは**できません**。 サイトを削除し、その URL を再利用する場合は、削除したサイトがまだ [[削除されたサイト](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)] の下に存在している場合があります。 URL を再利用するには、サイトを完全に削除する必要があります。 PowerShell を使ってサイトを完全に削除するには、[Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) コマンドレットの例を参照してください。
- 一部のユーザーはサイトを作成できない場合があります。 「[SharePoint Online のサイト作成を管理する](https://docs.microsoft.com/sharepoint/manage-site-creation)」を参照してください。
- サイトの**作成中**に、サイトが予想以上に長く停止しているように見えることがあります。 この問題が発生してから 24 時間以上経過した場合は、サポート チケットを記録してください。 多くの場合、すでに解決策に取り組んでいます。 解決策を完成させるために少なくとも 24 時間を与えてください。
