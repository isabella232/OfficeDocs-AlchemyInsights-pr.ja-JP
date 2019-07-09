---
title: SharePoint または OneDrive でアクセスを制限する
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223717"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePoint または OneDrive でアクセスを制限する

SharePoint Online/OneDrive サービスへのアクセスを制限するさまざまな方法があります。 以降、これらのさまざまなアクセス制限方法について説明します。 

**アクセス許可の制限**

SharePoint Online と OneDrive for Business で、アクセス権が必要なグループ/個人にのみアクセス権を付与することで、サイト、ファイル、フォルダーなどのアイテムへのアクセスを制限します。

- [SharePoint リストまたはライブラリのアクセス許可をカスタマイズする](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint サイト権限をカスタマイズする](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [サブフォルダーの権限の変更](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [非管理対象デバイスからのアクセスを制御する](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint 管理者または Office 365 のグローバル管理者は、非管理対象デバイス (ハイブリッド AD に参加していないデバイスまたは Intune 内の準拠していないデバイス) からの SharePoint および OneDrive のコンテンツに対するアクセスをブロックまたは制限することができます。

**ネットワークの場所の制限**

IT 管理者は、定義されている信頼できるネットワークの場所に基づいて、SharePoint と OneDrive のリソースへのアクセスを制御できます。 これは、場所に基づくポリシーとも呼ばれます。 詳細については、[「ネットワークの場所に基づいて SharePoint Online と OneDrive データへのアクセスを制御する」](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)を参照してください。

**サイト ロックの制限** 

SharePoint Online では、誰もアクセスできないようにサイト コレクションをロックできます。 これは、[Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState プロパティを使用して PowerShell および [SharePoint Online 管理シェル](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)を経由して設定されます。

**ユーザーがサイトまたはサブサイトを作成できないように制限する**

SharePoint 管理者または Office 365 グローバル管理者は、ユーザーが独自の SharePoint サイトを作成し管理できるようにし、ユーザーが作成できるサイトの種類を決定し、サイトの場所を指定することができます。 詳細については、[「SharePoint Online のサイト作成を管理する」](https://docs.microsoft.com/sharepoint/manage-site-creation)を参照してください。

