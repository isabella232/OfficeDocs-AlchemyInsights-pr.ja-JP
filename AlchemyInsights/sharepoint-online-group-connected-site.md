---
title: SharePoint サイトにグループを追加する
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507852"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>SharePoint Online で接続されたサイトを作成またはグループ化する際の問題

グループに接続されたサイトを作成または再作成するときに、いくつかの一般的な問題が発生しました。

 グループとその接続されたサイトを削除し、同じ URL を持つ別のサイトを作成したい場合は、以前のサイトを完全に削除する必要があります。

[Spo 管理シェル](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)をダウンロードする

 Powershell の概要については、「 [SharePoint Online 管理シェルの](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)概要」を参照してください。

[Remove-spodeletedsite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell コマンドレットを使用して、削除されたサイトからサイトを削除します。

グループに接続されたサイトを作成している場合に、同じエイリアスを持つ他のグループが既に存在する場合は、[管理センターから Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)の既存のグループを確認します。 この問題を解決するには、既存のグループが不要になった場合は削除し、別のエイリアスを割り当てたサイトを作成します。

SharePoint でモダングループを作成して使用するには、さまざまな方法があります。

既存のサイトを Office 365 グループに接続することができます。 詳細については、「 [Connect An Office 365 group using The SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)」を参照してください。

Office 365 グループに接続されたサイトを作成するには、チームサイトを作成する必要があります。 詳細については、「 [SharePoint でチームサイトを作成する](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)」を参照してください。

