---
title: Office ファイルをダブルクリックしても開くことができない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2020
ms.locfileid: "42575401"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="fa669-102">Office ファイルをダブルクリックしても開くことができない</span><span class="sxs-lookup"><span data-stu-id="fa669-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="fa669-103">Office ファイルをダブルクリックすると、プログラムが開かれているように見えますが、ファイル自体は開かれません。</span><span class="sxs-lookup"><span data-stu-id="fa669-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="fa669-104">または、「プログラムにコマンドを送信するときに問題が発生しました」というエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fa669-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="fa669-105">これには多くの原因がありますが、最も一般的なソリューションは次の2つです。</span><span class="sxs-lookup"><span data-stu-id="fa669-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="fa669-106">Excel で、[DDE] オプションがオフになっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="fa669-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="fa669-107">このオプションを確認するには、新しいブックを作成し、[**ファイル > オプション > Advanced**を選択します。</span><span class="sxs-lookup"><span data-stu-id="fa669-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="fa669-108">**[全般**] セクションで、[**動的データ交換 (DDE) を使用している他のアプリケーションを無視**する] をオフにします。</span><span class="sxs-lookup"><span data-stu-id="fa669-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="fa669-109">オンライン修復を実行して、既定の設定を復元します。</span><span class="sxs-lookup"><span data-stu-id="fa669-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="fa669-110">Windows の [スタート] ボタンをクリックし、[コントロールパネル] を検索します。</span><span class="sxs-lookup"><span data-stu-id="fa669-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="fa669-111">**コントロールパネル**を開き、[**プログラム > プログラムと機能**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="fa669-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="fa669-112">[ **Microsoft Office [バージョン]]** を右クリックし、[ **Change > Online Repair**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fa669-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="fa669-113">これらのソリューションのいずれも機能しない場合は、ソリューションの完全な一覧については、「サポート」の記事「 [Office ファイルをダブルクリックしても開く](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)ことができない」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa669-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
