---
title: Office ファイルをダブルクリックしても開かない
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
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812084"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="0b8ef-102">Office ファイルをダブルクリックしても開かない</span><span class="sxs-lookup"><span data-stu-id="0b8ef-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="0b8ef-103">Office ファイルをダブルクリックしたあとで、プログラムは開くことができても、ファイル自体が開かないことがあります。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="0b8ef-104">または、「プログラムにコマンドを送信しているときに、エラーが発生しました。」というエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="0b8ef-105">これらは多くの原因が考えられますが、一般的な解決策は次の 2 つです。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="0b8ef-106">Excel で、DDE オプションがオフになっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="0b8ef-107">このオプションを確認するには、新しいブックを作成し、**[ファイル] > [オプション] > [詳細設定]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="0b8ef-108">**[全般]** セクションの **[Dynamic Data Exchange (DDE) を使用する他のアプリケーションを無視する]** をオフにします。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="0b8ef-109">オンライン修復を実行して、既定の設定を復元します。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="0b8ef-110">Windows の [スタート] ボタンをクリックし、[コントロール パネル] を検索します。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="0b8ef-111">**[コントロール パネル]** を開き、**[プログラム] > [プログラムと機能]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="0b8ef-112">次に、**Microsoft Office [バージョン]** を右クリックし、**[変更] > [オンライン修復]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="0b8ef-113">これらの方法で解決しない場合は、サポート記事「[Office ファイルをダブルクリックしても開かない](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)」の中から解決策をお探しください。</span><span class="sxs-lookup"><span data-stu-id="0b8ef-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
