---
title: テナントの削除
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993898"
---
# <a name="delete-tenant"></a>テナントの削除

Azure AD を削除するには、次のことを確認してください。
- ディレクトリのグローバル管理者である。
- admin@contoso.onmicrosoft.com など、contoso.onmicrosoft.com などの既定のディレクトリを持つアカウントでサインインしていない。
- 削除する前に、アクティブなアプリケーションを削除します。 アクティブなアプリケーションを削除するには、[アプリの登録] に移動して既存のアプリケーションを削除します。
- ディレクトリに Microsoft Azure、Office 365、Azure AD Premium などの Microsoft Online Service のアクティブなサブスクリプションは関連付けられていません。 サブスクリプションを譲渡するか、Azure サポートと課金からアクティブなサブスクリプションのキャンセルを続行します。 Office 365 と Azure サブスクリプションをキャンセルする方法の詳細について説明します。 テナントへの既存のサブスクリプションの関連付けや追加に関するガイダンスについては、「[Azure サブスクリプションを Azure Active Directory テナントに関連付けるまたは追加する](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)」を参照してください。
- アクティブなライセンスはありません。 ライセンスを削除するには、「[サブスクリプションを削除してライセンスを削除する方法](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)」を参照してください。
- Azure AD を削除しようとした際、ディレクトリにはグローバル管理者であるあなた以外にアクティブなユーザーは見つかりませんでした。 その他のアクティブなユーザーを削除します。また、admin@contoso.com で作成されたユーザーなど、テナント内のカスタム ドメイン名の依存関係も削除する必要があります。

次のことを行うための詳細なステップ:
- "Azure Active Directory" または "サブスクリプション" を削除するには、「[Azure Active Directory を削除する](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)」を参照してください。
- ディレクトリ内のアプリケーションを削除するには、「[アプリケーションを削除する](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)」を参照してください。 
