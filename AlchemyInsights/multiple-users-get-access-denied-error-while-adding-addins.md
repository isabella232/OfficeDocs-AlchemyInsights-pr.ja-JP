---
title: Outlook でアドインを追加するときに、複数のユーザーにアクセス拒否エラーが発生する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065397"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Outlook でアドインを追加するときに、複数のユーザーにアクセス拒否エラーが発生する

組織のどの管理者に、Outlook 用のアドインをインストールして管理するアクセス許可を持たせるかを指定できます。また、組織のどのユーザーに、自分で使用するアドインをインストールして管理するアクセス許可を持たせるかを指定することもできます。

詳細については、[「Outlook 用のアドインをインストールおよび管理できる管理者とユーザーを指定する」](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins) をご覧ください。

ユーザーのアクセス許可が正常に割り当てられたことを確認するには、<Role Name> を検証するロールの名前に置き換え、Exchange Online PowerShell で次のコマンドを実行します:

Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers

この例は、組織のために Office ストアのアドインをインストールするのに必要なアクセス許可を割り当てた対象を確認する方法を示しています。

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

Get-ManagementRoleAssignment の結果の [有効なユーザー] 列のエントリを確認します。

構文およびパラメーターの詳細については、「[Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)」を参照してください。
 