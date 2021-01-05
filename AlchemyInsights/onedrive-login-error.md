---
title: One Drive ログイン エラー AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982624"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="dfea6-102">One Drive ログイン エラー AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="dfea6-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="dfea6-103">OneDrive アプリにサインインしたときに、「AADSTS50011: 要求で指定された返信 URL が返信と一致しません」というエラーが表示された場合は、次のことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="dfea6-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="dfea6-104">OneDrive のバージョンはバージョン 20.052.XXXX.XXXX 以上である必要があります。</span><span class="sxs-lookup"><span data-stu-id="dfea6-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="dfea6-105">バージョンを確認するには、通知領域で、青い OneDrive アイコンをクリックして、**[ヘルプと設定]、[設定]、[バージョン情報]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="dfea6-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="dfea6-106">ネットワークが **g.live.com** と **oneclient.sfx.ms** へのトラフィックをブロックする場合があります。</span><span class="sxs-lookup"><span data-stu-id="dfea6-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="dfea6-107">そのトラフィックがブロックされている場合、OneDrive は自動的に更新できません。</span><span class="sxs-lookup"><span data-stu-id="dfea6-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="dfea6-108">ネットワーク管理者と協力して、これらの URL にアクセスできるようにします。</span><span class="sxs-lookup"><span data-stu-id="dfea6-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="dfea6-109">[これらのエンドポイント](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide)は、Microsoft 365 プランを使用しているお客様にはアクセス可能である必要があります。</span><span class="sxs-lookup"><span data-stu-id="dfea6-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="dfea6-110">現在のバージョンの OneDrive を手動で取得する必要がある場合は、[https://aka.ms/getonedrive](https://aka.ms/getonedrive) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfea6-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
