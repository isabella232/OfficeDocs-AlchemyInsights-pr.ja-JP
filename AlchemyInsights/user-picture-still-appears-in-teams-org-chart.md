---
title: ユーザーの画像は引き続き Microsoft Teams の組織図に表示されます
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422387"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>ユーザーの画像は引き続き Microsoft Teams の組織図に表示されます

組織内の 1 人以上の個人が無効化または削除され、そのプロフィール写真が組織図に引き続き表示される場合は、**ShowInAddressLists** が False に設定されている可能性があります。 

1. Microsoft 365 管理センター > [[アクティブ ユーザー]](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) に移動し、写真がまだ表示されているユーザーを選択します。 
1. **[メール]** タブを選択し、**[グローバル アドレス一覧に表示]** が **[いいえ]** に設定されていることを確認します。

**ShowInAddressLists** を **[いいえ]** に設定できない場合は、次の項目を確認してください。 

- ユーザーが Exchange の受信者リストから表示される可能性があります。 詳細については、「[Exchange Onlineでアドレス一覧を管理する](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists)」を参照してください。 
- ユーザーが Azure Active Directory のアドレス一覧から表示される可能性があります。 詳細については「[Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)」を参照してください。 