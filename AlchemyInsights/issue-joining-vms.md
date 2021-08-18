---
title: VM への参加の問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: d89fb92ce1775e5a77808a1893a315419b4d54706dc737327c51f7c4c4e488e2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088077"
---
# <a name="issue-joining-vms"></a>VM への参加の問題

VM への参加中に発生する問題を解決するには、次の手順を実行します。

1. **SAMAccountName** 形式 (「CONTOSO\joeuser」) の代わりに **UPN** 形式 (たとえば、「joeuser@contoso.com」) を使用してサインインしてみてください。
2. *作業の開始* ガイドに記載されている手順に従って、パスワードの同期が有効になっていることを確認します。
3. 影響を受けるユーザー アカウントが Azure AD テナントの外部アカウントでないことを確認します。 Azure AD Domain Services には管理対象ドメインの資格情報がないため、外部ユーザーは管理対象ドメインにサインインできません。
4. 影響を受けるユーザー アカウントがクラウド専用のユーザー アカウントの場合は、Azure AD Domain Services を有効にした後でユーザーがパスワードを変更したことを確認します。 この手順により、Azure AD Domain Services に必要な資格情報ハッシュが生成されます。
5. 影響を受けるユーザー アカウントがオンプレミス ディレクトリから同期される場合は、Azure AD Connect の推奨リリースが完全同期を実行するように構成されていることを確認します。
6. 手順 4 を確認しても問題が解決しない場合は、同期マシンから次のコマンドを実行します。
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.