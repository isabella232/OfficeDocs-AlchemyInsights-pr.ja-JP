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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="f02a5-102">Bitlocker 回復キーにアクセスする</span><span class="sxs-lookup"><span data-stu-id="f02a5-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="f02a5-103">BitLocker 設定の Intune エンドポイント保護ポリシーを構成する場合、BitLocker 回復情報を Azure Active Directory に保存するかどうかを定義できます。</span><span class="sxs-lookup"><span data-stu-id="f02a5-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="f02a5-104">その設定が構成されている場合、保存された回復データは、Intune デバイス ブレードのデバイス レコード データの一部として Intune 管理者に対して、次の 2 つの方法で表示されます。</span><span class="sxs-lookup"><span data-stu-id="f02a5-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="f02a5-105">デバイス - Azure AD devices -> 「デバイス」またはデバイス -> すべてのデバイス -> 「デバイス」 -> 回復キー</span><span class="sxs-lookup"><span data-stu-id="f02a5-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="f02a5-106">または、デバイス自体に管理アクセス権がある場合は、管理者特権でのコマンド プロンプトから次のコマンドを実行して、回復キー (パスワード) を表示できます。</span><span class="sxs-lookup"><span data-stu-id="f02a5-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="f02a5-107">Intune に登録する前にデバイスが暗号化されていた場合は、OOBE プロセス中にデバイスにサインインするために使用される「Microsoftアカウント」 (MSA) に回復キーが関連付けられている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f02a5-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="f02a5-108">この場合、https://onedrive.live.com/recoverykey にアクセスしてその MSA でサインインすると、回復キーが保存されたデバイスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="f02a5-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="f02a5-109">デバイスがドメインベースのグループ ポリシーによる構成の結果として暗号化された場合、回復情報はオンプレミス Active Directory に保存されます。</span><span class="sxs-lookup"><span data-stu-id="f02a5-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

