---
title: Outlook でアドインが表示されない複数のユーザー
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729876"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="79e6c-102">Outlook でアドインが表示されない複数のユーザー</span><span class="sxs-lookup"><span data-stu-id="79e6c-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="79e6c-103">Outlook アドインをテストしても何も表示されない場合は、最初のトラブルシューティング手順として、\*\*Get-OrganizationConfig \*\* PowerShell コマンドレットを使用して_ AppsForOfficeEnabled _パラメータをクエリします。</span><span class="sxs-lookup"><span data-stu-id="79e6c-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="79e6c-104">クエリが\*\* False **の値を返す場合、** Set-OrganizationConfig **コマンドレットを使用してこのパラメーターを** True \*\*に設定すると、アドインが予想どおりに表示されます。</span><span class="sxs-lookup"><span data-stu-id="79e6c-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="79e6c-105">_AppsForOfficeEnabled_ パラメーターを\*\* False\*\* に設定することはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="79e6c-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="79e6c-106">値が\*\* False \*\*の場合、上記のすべての管理およびユーザーロール設定が上書きされ、組織内のユーザーが新しいアプリをアクティブ化できなくなります。</span><span class="sxs-lookup"><span data-stu-id="79e6c-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="79e6c-107">詳細については、「[Outlook 用のアドインをインストールおよび管理できる管理者とユーザーを指定する](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="79e6c-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>