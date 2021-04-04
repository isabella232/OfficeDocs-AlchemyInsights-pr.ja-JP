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
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505073"
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

回復キーを Azure Active Directory に格納するようにエンドポイント保護ポリシーを構成したが、特定のデバイスのキーがアップロードされていない場合は、MEM コンソールからそのデバイスの回復キーをローテーションすることでアップロードをトリガーできます。 詳細については、「[BitLocker 回復キーのローテーション](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)」を参照してください。

