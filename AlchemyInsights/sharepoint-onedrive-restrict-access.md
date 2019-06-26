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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223717"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePoint または OneDrive でアクセスを制限する

SharePoint Online/OneDrive サービスへのアクセスを制限するには、さまざまな方法があります。 これらのさまざまなアクセス制限方法について、以下に説明します。 

**アクセス許可の制限**

SharePoint Online と OneDrive for business では、アクセスを必要とするグループまたは個人へのアクセスのみを許可することによって、サイト、ファイル、フォルダーなどのアイテムへのアクセスを制限します。

- [SharePoint リストまたはライブラリのアクセス許可をカスタマイズする](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint サイト権限をカスタマイズする](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [サブフォルダーの権限の変更](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [非管理対象デバイスからのアクセスを制御する](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Office 365 の SharePoint またはグローバル管理者は、管理されていないデバイス (ハイブリッド AD に参加していないか、または Intune で準拠していないデバイス) からの SharePoint および OneDrive のコンテンツへのアクセスをブロックまたは制限することができます。

**ネットワークの場所の制限**

IT 管理者は、信頼できる定義済みのネットワークの場所に基づいて SharePoint および OneDrive リソースへのアクセスを制御できます。 これは、場所ベースのポリシーとも呼ばれます。 詳細については、「[ネットワークの場所に基づいて SharePoint Online および OneDrive データへのアクセスを制御する](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)」を参照してください。

**サイトロック制限** 

SharePoint Online では、サイトコレクションをロックダウンすることができます。アクセス権を持つユーザーはいません。 これは、PowerShell および[SharePoint Online 管理シェル](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)で[get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState プロパティを使用して設定されます。

**サイトまたはサブサイトの作成をユーザーに制限する**

SharePoint 管理者または Office 365 のグローバル管理者は、ユーザーが自分の SharePoint サイトを作成および管理したり、作成できるサイトの種類を決定したり、サイトの場所を指定したりすることができます。 詳細については、「 [SharePoint Online でサイト作成を管理](https://docs.microsoft.com/sharepoint/manage-site-creation)する」を参照してください。

