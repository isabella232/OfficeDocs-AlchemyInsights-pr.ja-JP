---
title: Outlook でアドインが表示されない複数のユーザー
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198643"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Outlook でアドインが表示されない複数のユーザー

Outlook アドインをテストしても何も表示されない場合は、最初のトラブルシューティング手順として、**Get-OrganizationConfig ** PowerShell コマンドレットを使用して_ AppsForOfficeEnabled _パラメータをクエリします。 クエリが** False **の値を返す場合、** Set-OrganizationConfig **コマンドレットを使用してこのパラメーターを** True **に設定すると、アドインが予想どおりに表示されます。

_AppsForOfficeEnabled_ パラメーターを** False** に設定することはお勧めしません。 値が** False **の場合、上記のすべての管理およびユーザーロール設定が上書きされ、組織内のユーザーが新しいアプリをアクティブ化できなくなります。

詳細については、「[Outlook 用のアドインをインストールおよび管理できる管理者とユーザーを指定する](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)」をご覧ください。