---
title: SharePoint または OneDrive 管理センターにアクセスできません
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824440"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>SharePoint または OneDrive 管理センターにアクセスできません

- SharePoint または OneDrive 管理センターがアクセス不可、あるいは利用できない場合、一時的なサービスの問題が発生している可能性があります。そのような状況では、ユーザーが SharePoint サイトまたは OneDrive コンテンツにアクセスする際に、一時的な遅延やナビゲーション エラーが発生する可能性があります。 [サービスの正常性ダッシュボード](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)を確認して、組織が影響を受けるかどうかを調べます。

- グローバル管理者と SharePoint 管理者には SharePoint のラインセンスが付与される必要があります。 新しく作成されたアカウントに SharePoint のライセンスまたは管理者の役割を割り当てた直後は、"アクセスが拒否されました" や "ユーザーが見つかりません" などのエラーが表示されて SharePoint にアクセスできない場合があります。 同期がシステム全体で完了するまで、少なくとも 24 時間お待ちください。 24 時間が長く感じられることは理解しております。 多くの場合、すでに解決策に取り組んでいます。

- Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) ユーザーは、許可されたアクセス時間枠が小さすぎる場合に、アクセス拒否となる時があります。「[PIM アカウントに対するアクセスが拒否される](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)」を参照してください。