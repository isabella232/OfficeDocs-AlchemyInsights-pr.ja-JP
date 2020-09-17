---
title: パブリック フォルダーにアクセスできません
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812552"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook はパブリック フォルダーに接続できません

パブリック フォルダー アクセスが一部のユーザーに対して機能しない場合には、以下を試してください。

EXO PowerShell に接続し、問題のあるユーザー アカウントの DefaultPublicFolderMailbox パラメーターを、動作中のユーザー アカウントのパラメーターと一致するように構成します。

例:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

変更が有効になるまで、少なくとも 1 時間待ちます。

問題が解決しない場合は、[この手順](https://aka.ms/pfcte)に従って、Outlook を使用したパブリック フォルダー アクセスの問題をトラブルシューティングしてください。
 
**Outlook を使用してパブリック フォルダーにアクセスできるユーザーを制御するには**:

1.  SSet-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $falseを使用する  
      
    $true: ユーザーに Outlook のパブリック フォルダーへのアクセスを許可します  
      
    $false: ユーザーが Outlook のパブリック フォルダーにアクセスできないようにします。 これが既定値です。  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**注**: この手順で制御できるのは、Windows クライアント用の Outlook デスクトップとの接続のみです。 ユーザーは OWA または Outlook for Mac を使用してパブリック フォルダーに引き続きアクセスできます。
 
詳細については、[Outlookでのパブリックフォルダーへの制御された接続のサポートについてのお知らせ](https://aka.ms/controlpf)を をご覧ください。