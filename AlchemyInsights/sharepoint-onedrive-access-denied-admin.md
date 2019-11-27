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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751281"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Sharepoint/OneDrive 管理センターで "アクセスが拒否されました" メッセージをトラブルシューティングする

Sharepoint/OneDrive 管理センターをブラウザーで参照しようとしたときに、アクセス拒否のメッセージが表示された場合は、[ユーザーへのライセンス割り当て](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)を確認してください。 ユーザーにライセンスが付与されている場合は、そのユーザーに管理センターへのアクセスを許可する[管理者の役割が割り当てられている](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)ことも確認してください。

この問題は、ユーザーの削除後に同じユーザー プリンシパル名 (UPN) でユーザーを再作成した場合にも発生することがあります。 新しいアカウントは、別の PUID (Passport 一意識別子) を使用して作成されます。 そのユーザーがサイト コレクションや自分の OneDrive にアクセスしようとしたときに、ユーザーの PUID は間違ったものになります。 もう 1 つのシナリオには、Active Directory 組織単位 (OU) とのディレクトリ同期が関連します。 SharePoint にサインインしているユーザーが、別の OU に移動されて SharePoint と再同期されると、この問題が発生することがあります。

この問題を解決するには、「[Office 365 でユーザーを復元する](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)」に記載された手順を実行して元の UPN を復元する必要があります。

注: それまでアクセスできていた複数のユーザーが OneDrive または SharePoint 管理センターを利用できない場合は、サービスに一時的な問題が発生している可能性があります。  [サービス正常性ダッシュボードを確認](https://portal.office.com/adminportal/home#/servicehealth)してください。


