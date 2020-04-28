---
title: ポータルで重複しているデバイス レコード
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "43791316"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="f0647-102">ポータルで重複しているデバイス レコード</span><span class="sxs-lookup"><span data-stu-id="f0647-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="f0647-103">ポータルで、1 つのデバイスに対して 2 つのレコードが表示されることがあります。これは、そのデバイスが共同管理の状態を Configuration Manager サイトに正しく報告していない場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="f0647-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="f0647-104">デバイスの共同管理の状態を調べるには、Configuration Manager コンソールでデバイスの **[共同管理]** 列を確認します。</span><span class="sxs-lookup"><span data-stu-id="f0647-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="f0647-105">この列が表示されていない場合は、任意の列見出しを右クリックして、リストから目的の列を選択することで追加できます。</span><span class="sxs-lookup"><span data-stu-id="f0647-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="f0647-106">[共同管理] の値は、**[はい]** になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0647-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="f0647-107">この値が **[いいえ]** の場合は、クライアント デバイスで Configuration Manager クライアント アプレットを起動して、[全般] タブで **[Co-management]** プロパティを確認します。</span><span class="sxs-lookup"><span data-stu-id="f0647-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="f0647-108">この値が **[Enabled]** の場合は、クライアントと管理ポイントとの通信に問題があることを示しています。</span><span class="sxs-lookup"><span data-stu-id="f0647-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="f0647-109">デバイスの **CcmMessaging.log** を確認して、可能性のある接続の問題を調査してください。</span><span class="sxs-lookup"><span data-stu-id="f0647-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="f0647-110">この値が **[Disabled]** のときに、デバイスが Intune で登録されている場合は、デバイスの **CoManagementHandler.log** を調べて、デバイスが共同管理ポリシーを受け取っていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="f0647-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
