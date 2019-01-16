---
title: 設定または変更するパブリック フォルダーのアクセス許可
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: d537f1446318f1507f52297e547789fdf246b322
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297585"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="65127-102">パブリック フォルダーのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="65127-102">Permissions and Public Folders</span></span>

<span data-ttu-id="65127-103">Exchange 管理センター (EAC)、Outlook を使用してパブリック フォルダーのアクセス許可を変更するか、PowerShell:</span><span class="sxs-lookup"><span data-stu-id="65127-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="65127-104">Outlook については、[ここをクリック](https://support.office.com/article/https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)します。</span><span class="sxs-lookup"><span data-stu-id="65127-104">For Outlook instructions, [click here](https://support.office.com/article/https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="65127-p101">EAC、手順については[この資料](https://support.office.com/article/https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1)を参照してください。をクリックすることができます[ここ](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx)に [EAC] に移動します。</span><span class="sxs-lookup"><span data-stu-id="65127-p101">For EAC, refer to [this article](https://support.office.com/article/https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="65127-p102">Powershell では、追加 PublicFolderClientPermission 内線番号を使用する方法について、[この資料](https://support.office.com/article/https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)を参照してください。Powershell の Exchange への接続を指示する場合をクリックして[ここ](https://support.office.com/article/https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)。</span><span class="sxs-lookup"><span data-stu-id="65127-p102">For Powershell, refer to [this article](https://support.office.com/article/https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. If you need instructions to connect to Exchange Powershell, click [here](https://support.office.com/article/https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="65127-p103">**外部のユーザーがメールが有効なパブリック フォルダーに電子メールを送信できない**理由がある場合、パブリック フォルダーのアクセス許可がないことに必要な外部の電子メール配信します。これを修正する手順に従って、Outlook[はここ](https://support.office.com/article/https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)、または PowerShell の指示[は、ここ](https://support.office.com/article/https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)です。</span><span class="sxs-lookup"><span data-stu-id="65127-p103">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery. You can fix this using the Outlook instructions [here](https://support.office.com/article/https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.office.com/article/https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

