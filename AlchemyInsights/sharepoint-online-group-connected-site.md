---
title: SharePoint サイトにグループを追加する
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771212"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>SharePoint でグループ接続されたサイトを作成する際の問題

1. グループ接続されたサイトを作成または再作成する際に発生する一般的な問題がいくつかあります。
グループおよびグループと接続されたサイトを削除し、同じ URL で新たにサイトを作成する場合は、以前のサイトを完全に削除する必要があります。

   - [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) をダウンロードする
   - PowerShell の使用を開始する方法の詳細については、「[SharePoint Online 管理シェルの使用を開始する](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)」を参照してください。
   - [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell コマンドレットを使用して、削除されたサイトからサイトを削除します。 グループ サイトを完全に削除するには、PowerShell が必要です。

1. グループ接続されたサイトを作成する際に、「**同じエイリアスのグループが既に存在しています**」という警告が表示される場合、[Microsoft 365 管理センター](https://admin.microsoft.com/AdminPortal/Home#/groups)で既存のグループを確認します。 この問題を解決するには、不要になった既存のグループを削除するか、異なるエイリアスを割り当ててサイトを作成します。

1. SharePoint でモダン グループを作成および使用するには、さまざまな方法があります。

   - 既存のサイトを Microsoft 365 グループに接続することができます。 詳細については、「[SharePoint ユーザー インターフェイスを使用して Microsoft 365 グループを接続する](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)」を参照してください。
   - Microsoft 365 のグループ接続されたサイトを作成するには、[チーム サイト](https://admin.microsoft.com/sharepoint)を作成する必要があります。
