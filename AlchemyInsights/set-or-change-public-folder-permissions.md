---
title: パブリック フォルダーのアクセス許可を設定または変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 3f891beeba8303b05d6730f608034e22b2bcdb92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36550160"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="80a30-102">アクセス許可とパブリック フォルダー</span><span class="sxs-lookup"><span data-stu-id="80a30-102">Permissions and Public Folders</span></span>

<span data-ttu-id="80a30-103">パブリック フォルダーのアクセス許可を、Outlook、Exchange 管理センター (EAC)、PowerShell を使用して変更することができます。</span><span class="sxs-lookup"><span data-stu-id="80a30-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="80a30-104">Outlook での手順については、[ここをクリック](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)してください。</span><span class="sxs-lookup"><span data-stu-id="80a30-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="80a30-p101">EAC での手順については、[この記事](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1)を参照してください。[ここ](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx)をクリックすると、EAC に移動することができます。</span><span class="sxs-lookup"><span data-stu-id="80a30-p101">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="80a30-p102">PowerShell で Add-PublicFolderClientPermission コマンドレットを使用する手順については、[この記事](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)を参照してください。Exchange PowerShell への接続方法については、[ここ](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)をクリックしてください。</span><span class="sxs-lookup"><span data-stu-id="80a30-p102">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="80a30-p103">**メールが有効なパブリック フォルダーに対して外部ユーザーがメールを送信できない場合**、外部メールの配信に必要なアクセス許可がパブリック フォルダーにないことが原因として考えられます。この問題を Outlook を使用して解決する手順については[こちら](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)、PowerShell を使用して解決する手順については[こちら](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80a30-p103">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery. You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

