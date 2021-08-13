---
title: パフォーマンスの問題 - SharePoint または OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093743"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint または OneDrive において、処理が遅い、アクセスできない、または複数のユーザーで使用できない

OneDrive または SharePoint サイトがアクセス権を持っている複数のユーザーから利用できない場合は、一時的なサービス上の問題が発生している可能性があります。[サービス正常性ダッシュボードを確認してください](https://portal.office.com/adminportal/home#/servicehealth)。

**ユーザーの追加とライセンス認証**

[一般法人向け Microsoft 365 のユーザーにライセンスが割り当てられている](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)ことを確認してください。


**アクセス許可の割り当て**

ユーザーに SharePoint ライセンスが割り当てられていてもアクセス拒否メッセージが表示される場合は、そのユーザーに[適切なアクセス許可レベルが割り当てられている](https://docs.microsoft.com/sharepoint/understanding-permission-levels)ことを確認してください。

**アクセス要求機能の使用を検討する**

[アクセス要求機能](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)は、ユーザーが表示する権限がないコンテンツへのアクセスを要求できるようにする機能です。

**カスタム スクリプトを許可するとアクセス拒否の問題が発生する可能性がある**

特定のシナリオでは、*カスタム スクリプトを許可* する機能を使用するとアクセス拒否が発生することがあります。 影響を受ける機能のリスト、セキュリティに関する考慮事項、この機能を無効にする方法については、 「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。

