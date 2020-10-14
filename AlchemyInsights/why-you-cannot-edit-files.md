---
title: ファイルが編集中にロックされる
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "9000123"
- "1622"
- "1713"
ms.openlocfilehash: 3020837e8e8dd3b9ff4ada33f23c6118e83c3806
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664499"
---
# <a name="why-cant-i-edit-files"></a><span data-ttu-id="59c85-102">ファイルを編集できないのはなぜですか。</span><span class="sxs-lookup"><span data-stu-id="59c85-102">Why can't I edit files?</span></span>

<span data-ttu-id="59c85-103">[ファイルを編集できない理由](https://support.office.com/article/why-can-t-i-edit-this-file-97315f48-aa5e-49d3-a4ae-a14b73daf87b)をいくつか見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="59c85-103">Take a quick look at some of the reasons [why you might not be able to edit the file](https://support.office.com/article/why-can-t-i-edit-this-file-97315f48-aa5e-49d3-a4ae-a14b73daf87b).</span></span>

<span data-ttu-id="59c85-104">**チェックアウト、必須**または**検証**の列またはメタデータを含むライブラリがある場合、または**下書きアイテムのセキュリティ**が**編集できるユーザーのみ**に設定されている場合、またはライブラリのバージョン設定で**アイテムを承認できるユーザーのみ**が対象となります。</span><span class="sxs-lookup"><span data-stu-id="59c85-104">If you have libraries with **Checkout, Required** or **Validation** columns or metadata, or when **Draft Item Security** is set to either **Only users who can edit** or **Only users who can approve items** in Version Settings of the library:</span></span>

- <span data-ttu-id="59c85-105">SharePoint ドキュメント ライブラリの場合、これらのアイテムは読み取り専用として同期されます。</span><span class="sxs-lookup"><span data-stu-id="59c85-105">For SharePoint document libraries, these items will be synchronized as read-only.</span></span>

- <span data-ttu-id="59c85-106">OneDrive ライブラリの場合、OneDrive では同期状態の横にロック アイコン (OneDrive ファイルのロック アイコン) が表示され、ユーザーは前述の設定が削除されるまでライブラリを同期できません。</span><span class="sxs-lookup"><span data-stu-id="59c85-106">For OneDrive libraries, OneDrive will show a lock icon ( OneDrive file locked icon ) next to the sync status and the user will not be able to synchronize the library until the mentioned settings have been removed.</span></span> 

<span data-ttu-id="59c85-107">Word または Excel のロックされたファイル関する詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59c85-107">For more information regarding locked files for Word or Excel, please reference the articles below.</span></span>

- [<span data-ttu-id="59c85-108">「Office ファイルの編集中に "アップロードに失敗しました" または "自動的に保存できませんでした" というエラーが表示される」</span><span class="sxs-lookup"><span data-stu-id="59c85-108">I got an "Upload failed" or "Couldn't save automatically" error while editing an Office file</span></span>](https://support.office.com/article/i-got-an-upload-failed-or-couldn-t-save-automatically-error-while-editing-an-office-file-93a14d34-88e3-4a91-9eef-58cc541d31f8)

- [<span data-ttu-id="59c85-109">Excel ファイルの編集が他のユーザーによってロックされている</span><span class="sxs-lookup"><span data-stu-id="59c85-109">Excel file is locked for editing by another user</span></span>](https://support.office.com/article/Excel-file-is-locked-for-editing-by-another-user-6fa93887-2c2c-45f0-abcc-31b04aed68b3)

- [<span data-ttu-id="59c85-110">Word ファイルの編集が他のユーザーによってロックされている</span><span class="sxs-lookup"><span data-stu-id="59c85-110">Word file is locked for editing by another user</span></span>](https://support.microsoft.com/help/313472/the-document-is-locked-for-editing-by-another-user-error-message-when)
