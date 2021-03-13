---
title: Linux コンピューターで MDATP の除外を構成および検証する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751313"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="fcf23-102">Linux コンピューターで MDATP の除外を構成および検証する</span><span class="sxs-lookup"><span data-stu-id="fcf23-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="fcf23-103">MDATP スキャンから、特定のファイル、フォルダー、プロセス、およびプロセスを開いたファイルを除外できます。</span><span class="sxs-lookup"><span data-stu-id="fcf23-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="fcf23-104">除外することで、お客様の組織に固有またはカスタマイズされたソフトウェアおよびファイルの誤検出を防止できます。</span><span class="sxs-lookup"><span data-stu-id="fcf23-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="fcf23-105">また、MDATP によるパフォーマンスの問題を軽減するためにも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="fcf23-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="fcf23-106">詳細については、「[Linux 用に MDATP の除外を構成および検証する](https://go.microsoft.com/fwlink/?linkid=2144517)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fcf23-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="fcf23-107">この記事で説明されている除外事項は、エンドポイントでの検出と対応 (EDR) など、Linux 用の MDATP の他の機能には適用されません。</span><span class="sxs-lookup"><span data-stu-id="fcf23-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="fcf23-108">この記事で説明されている方法を使用して除外したファイルは、EDR アラートやその他の検出機能をトリガーする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fcf23-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
