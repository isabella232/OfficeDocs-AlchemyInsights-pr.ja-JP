---
title: Microsoft 365 アプリのアドインの展開
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233539"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Microsoft 365 アプリのアドインの展開

一元展開は、組織内のユーザーおよびグループに Office アドインを展開するための推奨方法です。 アドインを展開するには、以下の手順に従います。

**注**: Office のアドインを個別のユーザーとしてインストールするには、「[Office プログラムでアドインを表示、管理、インストールする](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)」を参照してください。 また、Office ストア アドインの個別取得が有効になっていることを確認してください。 詳細については、「すべてのクライアントで Office ストアをオフにしてアドインのダウンロードを防止[する (Outlook を除く)」を参照してください](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)。

1. 一元展開を使用して、環境がアドインの展開の要件を満たしていることを確認します。 詳細については、[要件](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)を参照してください。
2. Microsoft 365 管理センターで [**設定**]  >  [**統合アプリ**]  >  [**アプリを取得**] の順に移動して、アドインを展開します。 

注: 

- 統合アプリでは、管理者がグローバル管理者または Exchange 管理者の権限を持っている必要があります。

- アドインを複数のユーザーに展開する場合は、個々のユーザーではなくグループを使用して割り当てを行うことをお勧めします。 詳細については、「[Considerations when assigning an add-in to users and groups (アドインをユーザーとグループに割り当てる際の考慮事項)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)」を参照してください。

- 一元展開は、ネストされたグループまたは親グループを持つグループのユーザーをサポートしていません。 詳細については、「[ユーザまたはグループへの割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)」を参照してください。

- ユーザーがサインインできるように、Microsoft 365 アプリ管理サービス (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') が有効になっていることを確認します。 詳細については、「 [アプリのプロパティを構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)」を参照してください。

- 統合アプリを使用したアドインの展開で問題が発生した場合は、[アドイン](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)を使用した展開をお試しください。

詳細については、以下を参照してください。

「[管理センターでアドインを展開する](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)」
「[管理センターでアドインを管理する](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)」
「[一元展開 PowerShell コマンドレットを使用してアドインを管理する](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)」
「[Microsoft 365 管理センターからの一元展開を使用した Microsoft アドインの発行](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)」
「[トラブルシューティング: ユーザーのアドインが表示されない](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)」
「[Office アドインでのユーザー エラーのトラブルシューティング](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)」