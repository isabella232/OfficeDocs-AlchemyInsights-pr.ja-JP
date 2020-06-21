---
title: 所有者は Outlook を使用してサブフォルダーを作成できない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749265"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="442c7-102">所有者は Outlook を使用してサブフォルダーを作成できない</span><span class="sxs-lookup"><span data-stu-id="442c7-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="442c7-103">**パブリック フォルダーの所有者が Outlook を使用してサブフォルダーを作成する場合、継続的な問題があります。この問題は間もなく修正されます。**</span><span class="sxs-lookup"><span data-stu-id="442c7-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="442c7-104">その間、次のいずれかの回避策を使用します。</span><span class="sxs-lookup"><span data-stu-id="442c7-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="442c7-105">問題はデスクトップ ウィンドウ (すべてのバージョン) の Outlook にのみ影響するため、Outlook for MAC を使用してサブフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="442c7-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="442c7-106">EXO シェルまたは EAC を使用してサブフォルダーを作成するように管理者に指示する</span><span class="sxs-lookup"><span data-stu-id="442c7-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="442c7-107">ユーザーの DefaultPublicFolderMailbox/EffectivePublicFolderMailbox を、問題の原因となっているフォルダーのコンテンツ メールボックス以外のメールボックスに変更します。</span><span class="sxs-lookup"><span data-stu-id="442c7-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="442c7-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="442c7-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="442c7-109">1 時間待って、Outlook クライアントを再起動します</span><span class="sxs-lookup"><span data-stu-id="442c7-109">Wait for an hour, restart outlook client</span></span>