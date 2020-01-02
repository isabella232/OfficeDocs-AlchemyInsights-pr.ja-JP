---
title: Bitlocker 回復キー
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/30/2019
ms.locfileid: "40923554"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Bitlocker 回復キーへのアクセス

Bitlocker 設定 Intune Endpoint Protection ポリシーを構成する場合は、Azure Active Directory に Bitlocker 回復情報を格納するかどうかを定義できます。

この設定が構成されている場合は、次の2つの方法で、intune デバイスブレードのデバイスレコードデータの一部として、保存された回復データを Intune 管理者に表示する必要があります。

Devices-Azure AD devices-> "デバイス" またはデバイス-> すべてのデバイス-> "デバイス"-> の回復キー

または、デバイス自体への管理アクセス権がある場合は、昇格したコマンドプロンプトから次のコマンドを実行することによって、回復キー (パスワード) を確認できます。

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
デバイスが Intune で enrolment より前に暗号化されている場合、回復キーは、OOBE プロセス中にデバイスへのサインインに使用される "Microsoft アカウント" (MSA) に関連付けられている可能性があります。 その場合は、その MSA をhttps://onedrive.live.com/recoverykey使用してアクセスおよびサインインすることにより、回復キーが保存されたデバイスを表示する必要があります。
 
ドメインベースのグループポリシーによって構成の結果としてデバイスが暗号化されている場合、回復情報は社内 Active Directory に格納されることがあります。
 

