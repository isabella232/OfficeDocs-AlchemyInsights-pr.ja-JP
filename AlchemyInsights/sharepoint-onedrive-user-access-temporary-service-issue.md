---
title: パフォーマンスの問題 - SharePoint または OneDrive
ms.author: pebaum
author: pebaum
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: f52f09ba9688bfc6dc932427fe950c0fc17a6f95
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642077"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint または OneDrive において、処理が遅い、アクセスできない、または複数のユーザーで使用できない

それまでアクセスできていた複数のユーザーが OneDrive または SharePoint のサイトを利用できない場合は、サービスに一時的な問題が発生している可能性があります。 [サービス正常性ダッシュボードを確認](https://portal.office.com/adminportal/home#/servicehealth)してください。

**ユーザーの追加とライセンス認証**

[Microsoft 365 for business のユーザーにライセンスを割り当てる](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)ようにしてください。


**アクセス許可の割り当て**

ユーザーに SharePoint ライセンスが割り当てられていてもアクセス拒否メッセージが表示される場合は、そのユーザーに[適切なアクセス許可レベルが割り当てられている](https://docs.microsoft.com/sharepoint/understanding-permission-levels)ことを確認してください。

**アクセス要求機能の使用を検討する**

[アクセス要求機能](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)は、ユーザーが表示する権限がないコンテンツへのアクセスを要求できるようにする機能です。

**カスタム スクリプトを許可するとアクセス拒否の問題が発生する可能性がある**

特定のシナリオでは、*カスタム スクリプトを許可*する機能を使用するとアクセス拒否が発生することがあります。 影響を受ける機能のリスト、セキュリティに関する考慮事項、この機能を無効にする方法については、 「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。

