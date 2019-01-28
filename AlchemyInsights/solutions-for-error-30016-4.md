---
title: エラー 30016-4 の解決方法
ms.author: janellem
author: janellem
manager: scotv
ms.date: 12/19/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 21644564-4ba5-4537-abd3-9ac2dfe2ee47
ms.openlocfilehash: 38079f76eb410592e48d93409e705faa9788fe19
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476662"
---
# <a name="solutions-for-error-30016-4"></a><span data-ttu-id="21cb5-102">エラー 30016-4 の解決方法</span><span class="sxs-lookup"><span data-stu-id="21cb5-102">Solutions for error 30016-4</span></span>

<span data-ttu-id="21cb5-103">コンピューターから Office 365 ProPlus をアンインストールしようとすると、次のエラー メッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="21cb5-103">When you try to uninstall Office 365 ProPlus from a computer, you might receive the following error message:</span></span>
  
> <span data-ttu-id="21cb5-104">「問題が発生しました 30016-4」</span><span class="sxs-lookup"><span data-stu-id="21cb5-104">"Something went wrong 30016-4"</span></span>
    
<span data-ttu-id="21cb5-105">この問題は、**%temp%** ドライブが **%ProgramFiles%** 以外のドライブにマップされているときに発生します。</span><span class="sxs-lookup"><span data-stu-id="21cb5-105">This issue occurs if the **%temp%** drive is mapped to a drive other than **%ProgramFiles%**.</span></span> 
  
<span data-ttu-id="21cb5-106">問題を修正する場合は、コンピューターから Office を完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="21cb5-106">To fix, completely remove Office from the computer.</span></span>
  
1. <span data-ttu-id="21cb5-107">[サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)をダウンロードしてインストールします。</span><span class="sxs-lookup"><span data-stu-id="21cb5-107">Download and install the [Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span></span>
    
2. <span data-ttu-id="21cb5-108">起動後に、**[Office 製品のアンインストール]** からアンインストールするバージョンを選択して **[次へ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="21cb5-108">When it opens, from **Uninstall Office products** select the version you want to uninstall and select **Next**.</span></span> 
    
3. <span data-ttu-id="21cb5-109">各画面の操作を続行して、プロンプトが表示されたらコンピューターを再起動します。</span><span class="sxs-lookup"><span data-stu-id="21cb5-109">Continue going through screens and restart your computer when prompted.</span></span>
    
    <span data-ttu-id="21cb5-110">再起動後に、サポート/回復アシスタントが自動的に再開してアンインストール処理を完了します。</span><span class="sxs-lookup"><span data-stu-id="21cb5-110">After restarting, the Support and Recovery Assistant automatically re-opens to complete the uninstall process.</span></span>
    
4. <span data-ttu-id="21cb5-111">その後のプロンプトに従って、Office を再インストールするか、アシスタントを閉じます。</span><span class="sxs-lookup"><span data-stu-id="21cb5-111">Follow remaining prompts, and reinstall Office or close the assistant.</span></span>
    

