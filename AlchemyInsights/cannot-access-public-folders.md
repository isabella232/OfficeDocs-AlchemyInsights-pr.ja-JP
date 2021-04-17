---
title: パブリック フォルダーにアクセスできません
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819517"
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