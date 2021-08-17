---
title: 1 名のユーザーが Outlook でアドインを表示しない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050663"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>1 名のユーザーが Outlook でアドインを表示しない

ユーザーは、正しい AppsForOfficeEnabled パラメーターがない役割の一部である可能性があります。 このコマンドレットを実行して、正しい役割がユーザーに関連付けられているかどうかを確認します。

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

詳細については、「[Outlook のアドインをインストールして管理できる管理者とユーザーを指定する](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)」を参照してください。
