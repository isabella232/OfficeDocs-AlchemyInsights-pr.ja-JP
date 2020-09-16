---
title: Outlook でアドインが表示されない複数のユーザー
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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729876"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Outlook でアドインが表示されない複数のユーザー

Outlook アドインをテストしても何も表示されない場合は、最初のトラブルシューティング手順として、**Get-OrganizationConfig ** PowerShell コマンドレットを使用して_ AppsForOfficeEnabled _パラメータをクエリします。 クエリが** False **の値を返す場合、** Set-OrganizationConfig **コマンドレットを使用してこのパラメーターを** True **に設定すると、アドインが予想どおりに表示されます。

_AppsForOfficeEnabled_ パラメーターを** False** に設定することはお勧めしません。 値が** False **の場合、上記のすべての管理およびユーザーロール設定が上書きされ、組織内のユーザーが新しいアプリをアクティブ化できなくなります。

詳細については、「[Outlook 用のアドインをインストールおよび管理できる管理者とユーザーを指定する](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)」をご覧ください。