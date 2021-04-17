---
title: MC210173 - SharePoint Designer の新しいユーザー設定フォーム機能の廃止
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831811"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="3c66a-102">MC210173 - SharePoint Designer の新しいユーザー設定フォーム機能の廃止</span><span class="sxs-lookup"><span data-stu-id="3c66a-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="3c66a-103">Sharepoint Online 内で[ユーザー設定 フォームを作成する](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2)に対して、SharePoint Designer の機能に影響する問題が特定されました。</span><span class="sxs-lookup"><span data-stu-id="3c66a-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="3c66a-104">慎重に調査したところ、この問題の修正はありませんが、2020 年 4 月 25 日 土曜日 午前 3 時 UTC 現在をもって、ユーザー設定のフォームの作成機能を無効を選択することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3c66a-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="3c66a-105">この変更は、以前に作成したフォームや、SharePoint Online デザイナーのその他の既存の機能を編集するのに影響はありません。</span><span class="sxs-lookup"><span data-stu-id="3c66a-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="3c66a-106">この変更を行うと、新しいフォームを作成するときに、"サーバーに変更を保存できませんでした" というエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3c66a-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="3c66a-107">ユーザー設定のフォームを作成するのに以前 SharePoint Designer を活用していたユーザーは、代わりにこの目的のために[PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="3c66a-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="3c66a-108">PowerApps は、SharePoint Online の最新の機能を操作しているユーザーが、ブラウザー ウィンドウから SharePoint リストおよびドキュメント ライブラリのユーザー設定フォームを作成および編集できる、簡単で強力なツールです。</span><span class="sxs-lookup"><span data-stu-id="3c66a-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="3c66a-109">PowerApps では、従来のコーディング知識や、InfoPath など任意の追加のアプリのダウンロードは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="3c66a-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="3c66a-110">**注** SharePoint Online の従来のユーザーは、PowerApps にアクセスして使用するために、最新のエクスペリエンスに一時的に切り替える必要があります。ただし、PowerApps で作成されるすべてのユーザー設定フォームには、SharePoint Online のクラシック エクスペリエンス ユーザーがアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="3c66a-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
