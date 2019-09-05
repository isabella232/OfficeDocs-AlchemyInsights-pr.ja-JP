---
title: "\"アクセスが拒否されました\" メッセージのトラブルシューティング"
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751281"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Sharepoint/OneDrive 管理センターでのアクセス拒否メッセージのトラブルシューティング

Sharepoint/OneDrive 管理センターを参照しようとしたときにアクセス拒否メッセージを受信した場合は、[ユーザーにライセンスを割り当てる](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)必要があります。 ユーザーがライセンスを持っている場合は、管理センターにアクセスできる[管理者の役割が割り当てら](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)れていることも確認してください。

この問題は、ユーザーを削除して、同じユーザープリンシパル名 (UPN) を使用して再作成した場合にも発生する可能性があります。 新しいアカウントは、異なる PUID (Passport の一意の ID) 値を使用して作成されます。 ユーザーがサイトコレクションまたは OneDrive にアクセスしようとすると、ユーザーの誤った PUID が表示されます。 2番目のシナリオでは、Active Directory の組織単位 (OU) とのディレクトリ同期が必要になります。 ユーザーが既に SharePoint にサインインしていて、別の OU に移動して SharePoint と resynced した場合、この問題が発生する可能性があります。

この問題を解決するには、記事「 [Office 365 でユーザーを復元](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)する」の手順に従って元の UPN を復元する必要があります。

注: 以前にアクセスしたことがある複数のユーザーが OneDrive または SharePoint 管理センターを使用できない場合は、一時的なサービスの問題が発生する可能性があります。  [サービス正常性ダッシュボードをチェックし](https://portal.office.com/adminportal/home#/servicehealth)ます。


