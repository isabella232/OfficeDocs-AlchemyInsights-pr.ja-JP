---
title: 646 AADConnect の構成方法
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963648"
---
# <a name="configure-sync-features"></a>同期機能を構成する

Azure AD Connect には、既定で有効になる、または、後で有効にできるいくつかの機能が含まれています。環境によっては、機能に追加の構成が必要な場合があります。

- [フィルター処理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)は、オブジェクトが Azure AD に同期されるように制限します。既定で、すべてのユーザー、連絡先、グループ、および Windows 10 コンピューター アカウントが同期されます。ドメイン、OU、またはその他の属性に基づいてオブジェクトを包含または除外できます。

- [パスワード ハッシュ同期](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)は、パスワード ハッシュをオンプレミス Active Directory から Azure AD に同期します。これにより、1 か所でパスワードを管理し、オンプレミス環境とクラウド環境の両方で同じパスワードを使用できるようになります。Active Directory は権限を持っているソースのため、独自のパスワード ポリシーを使用できます。

- [セルフ サービスによるパスワードのリセット (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) を使用すれば、ユーザーは、オンプレミス パスワード ポリシーを適用しながら、クラウドで独自のパスワードをリセットすることができます。

- [デバイスの書き戻し](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)を使用すれば、Azure AD に登録されているデバイスをオンプレミス Active Directory に書き戻すことができるため、条件付きアクセスに使用できるようになります。

- [偶発的削除の防止](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)は、同時オブジェクト削除が頻発 (同期あたり 500 を超えるオブジェクトの削除) しないように既定で有効になります。この設定は、組織のニーズに合わせて変更することができます。

- [自動アップグレード](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)は、高速インストール用に既定で有効になり、Azure AD Connect のバージョンが常に最新であることの保証を支援します。
