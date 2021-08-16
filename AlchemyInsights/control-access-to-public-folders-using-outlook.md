---
title: Outlook を使用してパブリック フォルダーへのアクセスを制御する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032563"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Outlook を使用してパブリック フォルダーへのアクセスを制御する

Outlook を使用してパブリック フォルダーにアクセスできるユーザーを制御するには:

1. `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` を使う

$true: ユーザーに Outlook のパブリック フォルダーへのアクセスを許可します  
$false: ユーザーが Outlook のパブリック フォルダーにアクセスできないようにします。 これが既定値です。  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

注: この手順で制御できるのは、Windows クライアントの Outlook デスクトップとの接続のみです。 ユーザーは OWA または Outlook for Mac を使用してパブリック フォルダーに引き続きアクセスできます。

詳細については、「[Outlook のパブリック フォルダーへの制御された接続](https://aka.ms/controlpf)」を参照してください。
