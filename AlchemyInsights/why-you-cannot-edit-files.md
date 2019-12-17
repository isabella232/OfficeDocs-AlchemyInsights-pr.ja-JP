---
title: ファイルが編集中にロックされる
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "9000123"
- "1622"
- "1713"
ms.openlocfilehash: 3ac4abe4d48e2feb887dc0945434ec26c19a2cf6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049414"
---
# <a name="why-cant-i-edit-files"></a><span data-ttu-id="d4853-102">ファイルを編集できないのはなぜですか。</span><span class="sxs-lookup"><span data-stu-id="d4853-102">Why can't I edit files?</span></span>

<span data-ttu-id="d4853-103">Windows デスクトップ アプリケーションでドキュメント、ワークシート、またはプレゼンテーションが編集のためにロックされていて開けない場合、そのファイルは別のユーザーが既に編集しているか、ファイルをチェックアウトしている可能性があります。ここでは、[ファイルの編集ができない理由](https://support.office.com/article/why-can-t-i-edit-this-file-97315f48-aa5e-49d3-a4ae-a14b73daf87b)のいくつかについて簡単に説明します。</span><span class="sxs-lookup"><span data-stu-id="d4853-103">If a document, worksheet, or presentation is locked for editing and can't be opened in the Windows desktop applications, it may be that the file is already being edited by someone else, or they have the file checked out. Let's take a quick look at some of the reasons [why you might not be able to edit the file](https://support.office.com/article/why-can-t-i-edit-this-file-97315f48-aa5e-49d3-a4ae-a14b73daf87b).</span></span>

<span data-ttu-id="d4853-104">**チェックアウト、必須**または**検証**の列またはメタデータを含むライブラリがある場合、または**下書きアイテムのセキュリティ**が**編集できるユーザーのみ**に設定されている場合、またはライブラリのバージョン設定で**アイテムを承認できるユーザーのみ**が対象となります。</span><span class="sxs-lookup"><span data-stu-id="d4853-104">If you have libraries with **Checkout, Required** or **Validation** columns or metadata, or when **Draft Item Security** is set to either **Only users who can edit** or **Only users who can approve items** in Version Settings of the library:</span></span>

- <span data-ttu-id="d4853-105">SharePoint ドキュメント ライブラリの場合、これらのアイテムは読み取り専用として同期されます。</span><span class="sxs-lookup"><span data-stu-id="d4853-105">For SharePoint document libraries, these items will be synchronized as read-only.</span></span>

- <span data-ttu-id="d4853-106">OneDrive ライブラリの場合、OneDrive では同期状態の横にロック アイコン (OneDrive ファイルのロック アイコン) が表示され、ユーザーは前述の設定が削除されるまでライブラリを同期できません。</span><span class="sxs-lookup"><span data-stu-id="d4853-106">For OneDrive libraries, OneDrive will show a lock icon ( OneDrive file locked icon ) next to the sync status and the user will not be able to synchronize the library until the mentioned settings have been removed.</span></span> 

<span data-ttu-id="d4853-107">Word または Excel のロックされたファイル関する詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4853-107">For more information regarding locked files for Word or Excel, please reference the articles below.</span></span>

- [<span data-ttu-id="d4853-108">Excel ファイルの編集が他のユーザーによってロックされている</span><span class="sxs-lookup"><span data-stu-id="d4853-108">Excel file is locked for editing by another user</span></span>](https://support.office.com/article/Excel-file-is-locked-for-editing-by-another-user-6fa93887-2c2c-45f0-abcc-31b04aed68b3)

- [<span data-ttu-id="d4853-109">Word ファイルの編集が他のユーザーによってロックされている</span><span class="sxs-lookup"><span data-stu-id="d4853-109">Word file is locked for editing by another user</span></span>](https://support.microsoft.com/help/313472/the-document-is-locked-for-editing-by-another-user-error-message-when)

