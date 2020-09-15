---
title: Bitlocker 回復キー
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685891"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Bitlocker 回復キーにアクセスする

BitLocker 設定の Intune エンドポイント保護ポリシーを構成する場合、BitLocker 回復情報を Azure Active Directory に保存するかどうかを定義できます。

その設定が構成されている場合、保存された回復データは、Intune デバイス ブレードのデバイス レコード データの一部として Intune 管理者に対して、次の 2 つの方法で表示されます。

デバイス - Azure AD devices -> 「デバイス」またはデバイス -> すべてのデバイス -> 「デバイス」 -> 回復キー

または、デバイス自体に管理アクセス権がある場合は、管理者特権でのコマンド プロンプトから次のコマンドを実行して、回復キー (パスワード) を表示できます。

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Intune に登録する前にデバイスが暗号化されていた場合は、OOBE プロセス中にデバイスにサインインするために使用される「Microsoftアカウント」 (MSA) に回復キーが関連付けられている可能性があります。 この場合、https://onedrive.live.com/recoverykey にアクセスしてその MSA でサインインすると、回復キーが保存されたデバイスが表示されます。
 
デバイスがドメインベースのグループ ポリシーによる構成の結果として暗号化された場合、回復情報はオンプレミス Active Directory に保存されます。
 

