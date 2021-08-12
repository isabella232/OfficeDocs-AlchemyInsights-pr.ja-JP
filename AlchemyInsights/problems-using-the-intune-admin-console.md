---
title: Intune 管理コンソールの使用に関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944136"
---
# <a name="problems-using-the-intune-admin-console"></a>Intune 管理コンソールの使用に関する問題

**Intune 管理コンソール内を移動すると、"アクセスが拒否されました" と表示されます。**

- Intune カスタム ロールのメンバーである場合は、Intune ライセンスまたは Enterprise Mobility Suite (EMS) ライセンスが自分のアカウントに割り当てられていることを確認します。
- Configuration Manager を使用してデバイスを管理している場合、自分が Configuration Manager MDM の Intune ユーザー コレクションに含まれていないことを確認します。
- Intune のロール ブレードで、適切なロールベースの管理制御 (RBAC) が自分に割り当てられていることを確認します。
- 使用しているグループが配布リストではないことを確認します。 Azure ポータルの Intune では、Azure Active Directory セキュリティ グループに属するユーザー アカウントのみがサポートされています。 自分のグループを確認するために、Azure ポータル > [**Intune**] > [**グループ**] または Azure ポータル > [**Azure Active Directory**] の順に移動します。

**ユーザーに割り当てられているアクセス権限の数が、割り当てられている Intune のロールに対して多すぎる**

ユーザーに、[**Intune**] > [**Intune のロール**] > [**自分のアクセス権限**] > [**エクスポート**] の順に移動して、付与されているアクセス許可を確認するよう依頼します。

**ロールにスコープ グループを追加しましたが、そのロールのユーザーには他のユーザーまたはデバイスが表示されます。**

スコープ グループは、ユーザーやデバイスを除外しません。スコープ グループ:

- ユーザーがポリシーまたはアプリケーションを割り当てる相手のユーザーを制限します。
- 特定のユーザーのみがデバイスでリモート タスクを実行できるようにします。

スコープ グループの詳細については、「[Microsoft Intune のロールベースのアクセス制御 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)」を確認してください。

**ユーザーを Intune のロールに追加しましたが、このユーザーは引き続き Intune 管理コンソールにフルアクセスできます。**

Azure ポータルで [Intune]、[**ユーザー**] の順に移動し、このユーザーが Azure ポータルで次のいずれのロールにも割り当てられていないことを確認します。

- 全体管理者
- Intune サービス管理者
- SharePoint 管理者

詳細については、「[Microsoft Intune のロールベースのアクセス制御 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)」を確認してください。

**アクセスに関する問題**

詳細については、「[Office 365、Azure、または Intune にサインインできない](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)」を参照してください。