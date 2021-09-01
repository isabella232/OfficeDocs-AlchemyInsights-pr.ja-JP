---
title: Microsoft Teams 組織図にユーザー画像が表示されない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/23/2021
ms.locfileid: "58793107"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Microsoft Teams 組織図にユーザー画像が表示されない

組織内の 1 人以上の個人が組織図にプロフィール写真がない場合、**ShowInAddressLists** の設定が **False** に設定されている可能性があります。

1. [Microsoft 365 管理センター]、[**[アクティブなユーザー]**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) の順に移動し、写真が見つからないユーザーを選択します。 
1. [**メール**] タブを選択し、**[グローバル アドレス一覧に表示]** が **[はい]** に設定されていることを確認します。 

**ShowInAddressLists** を **[はい]** に設定できない場合は、次の項目を確認してください。

- ユーザーが Exchange の受信者リストから非表示になっている可能性があります。 詳細については、[「Exchange Onlineでアドレス一覧を管理する」](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists)を参照してください。 
- ユーザーが Azure Active Directory のアドレス一覧から非表示になっている可能性があります。 詳細については「[Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)」を参照してください。 
