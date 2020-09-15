---
title: 印刷スプーラーの問題が解決されました
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801846"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="077a6-102">印刷スプーラーの問題が解決されました</span><span class="sxs-lookup"><span data-stu-id="077a6-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="077a6-103">使用しているデバイスが Windows 10 **OS Build 19041.329**で更新されていた場合、特定のプリンターで印刷できないという問題が発生している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="077a6-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="077a6-104">印刷しようとすると、エラーが発生するか、予期せず終了することがあります。また、プリンターからの出力はありません。</span><span class="sxs-lookup"><span data-stu-id="077a6-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="077a6-105">この問題は、OS ビルド **19041.331**、[KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523) で解決されています。</span><span class="sxs-lookup"><span data-stu-id="077a6-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="077a6-106">**調査継続中**</span><span class="sxs-lookup"><span data-stu-id="077a6-106">**Ongoing investigation**</span></span>

<span data-ttu-id="077a6-107">一部のデバイスでは、ローカル セキュリティ機関サブシステム サービス (LSASS) ファイル (**Isass.exe**) が失敗し、次のエラー メッセージが表示されることがあります。「重要なシステム プロセス C:\WINDOWS\system32\Isass.exe に失敗しました (状態コード: c0000008)。</span><span class="sxs-lookup"><span data-stu-id="077a6-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="077a6-108">コンピューターを再起動する必要があります。」</span><span class="sxs-lookup"><span data-stu-id="077a6-108">The machine must now be restarted".</span></span>  <span data-ttu-id="077a6-109">**マイクロフトは解決方法に取り組んでおり、今後のリリースで更新プログラムを提供します。**</span><span class="sxs-lookup"><span data-stu-id="077a6-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="077a6-110">詳細については、「[Windows 10 Version 2004 に関する既知の問題](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="077a6-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>