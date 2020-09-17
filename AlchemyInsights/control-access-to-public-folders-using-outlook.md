---
title: Outlook を使用してパブリック フォルダーへのアクセスを制御する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804405"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Outlook を使用してパブリック フォルダーへのアクセスを制御する

Outlook を使用してパブリック フォルダーにアクセスできるユーザーを制御するには:

1. `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` を使う

$true: ユーザーに Outlook のパブリック フォルダーへのアクセスを許可します  
$false: ユーザーが Outlook のパブリック フォルダーにアクセスできないようにします。 これが既定値です。  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

注: この手順で制御できるのは、Windows クライアントの Outlook デスクトップとの接続のみです。 ユーザーは OWA または Outlook for Mac を使用してパブリック フォルダーに引き続きアクセスできます。

詳細については、「[Outlook のパブリック フォルダーへの制御された接続](https://aka.ms/controlpf)」を参照してください。
