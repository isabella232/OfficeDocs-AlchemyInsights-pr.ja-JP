---
title: SharePoint と OneDrive でのバージョン管理
ms.author: efrene
author: efrene
ms.date: 8/07/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.custom:
- "5300025"
- "1702"
ms.openlocfilehash: 9c1ffe8c384a76d3df425623285fa4f9ebf757f2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503964"
---
# <a name="versioning-in-sharepoint-and-onedrive"></a><span data-ttu-id="4cd7c-102">SharePoint と OneDrive でのバージョン管理</span><span class="sxs-lookup"><span data-stu-id="4cd7c-102">User permissions in SharePoint and OneDrive</span></span> 


<span data-ttu-id="4cd7c-103">SharePoint リストまたはライブラリでバージョン管理が有効になっていると、リスト内のアイテムやライブラリ内のファイルのすべての変更を保存、追跡、および復元できるようになります。</span><span class="sxs-lookup"><span data-stu-id="4cd7c-103">When versioning is enabled in your SharePoint list or library, you can store, track, and restore items in a list and files in a library whenever they change.</span></span> <span data-ttu-id="4cd7c-104">バージョン管理とその他の設定 (チェックアウトなど) を組み合わせると、サイトに投稿されているコンテンツを詳細に管理できます。古いバージョンのアイテムまたはファイルの参照や復元が必要になったときに、その重要性がわかります。</span><span class="sxs-lookup"><span data-stu-id="4cd7c-104">Versioning, combined with other settings, such as checkout, gives you a lot of control of the content that is posted on your site and can provide real value if you ever have a need to look at or restore an old version of an item or file.</span></span>

<span data-ttu-id="4cd7c-105">バージョン管理の詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4cd7c-105">For more information on versioning please visit the below articles.</span></span>

- [<span data-ttu-id="4cd7c-106">SharePoint リストまたはライブラリでのバージョン管理のしくみ</span><span class="sxs-lookup"><span data-stu-id="4cd7c-106">How does versioning work in a list or library?</span></span>](https://support.office.com/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247)

- [<span data-ttu-id="4cd7c-107">リストまたはライブラリのバージョン管理を有効にし、構成する</span><span class="sxs-lookup"><span data-stu-id="4cd7c-107">Enable and configure versioning for a list or library</span></span>](https://support.office.com/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f&amp;ui=en-US&amp;rs=en-US&amp;ad=US)

- [<span data-ttu-id="4cd7c-108">バージョン履歴の表示方法</span><span class="sxs-lookup"><span data-stu-id="4cd7c-108">How to view version history</span></span>](https://support.office.com/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1)

- [<span data-ttu-id="4cd7c-109">OneDrive で以前のバージョンのファイルを復元する</span><span class="sxs-lookup"><span data-stu-id="4cd7c-109">Restore a previous version of a file in OneDrive</span></span>](https://support.office.com/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893?ui=en-US&amp;rs=en-US&amp;ad=US)

- [<span data-ttu-id="4cd7c-110">以前のバージョンの Office ファイルを表示する</span><span class="sxs-lookup"><span data-stu-id="4cd7c-110">View previous versions of Office files</span></span>](https://support.office.com/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2)

- [<span data-ttu-id="4cd7c-111">バージョン管理の制限</span><span class="sxs-lookup"><span data-stu-id="4cd7c-111">Versioning limits</span></span>](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)

>[!Note] 
><span data-ttu-id="4cd7c-112">Office 365 ユーザーの場合は、新しい OneDrive for Business のライブラリを作成すると、規定でバージョン管理がオンになるようになりました。しかも、ドキュメントの最新 500 バージョンが自動的に保存されます。</span><span class="sxs-lookup"><span data-stu-id="4cd7c-112">If you are an Office 365 customer, versioning is now turned on by default when you create new OneDrive for Business libraries, and it will automatically save the last 500 versions of a document.</span></span> <span data-ttu-id="4cd7c-113">これは、重要なドキュメントやデータの損失防止に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4cd7c-113">This will help you prevent losing important documents or data.</span></span> <span data-ttu-id="4cd7c-114">OneDrive for Business サイトやチーム サイトに、バージョン管理が有効になっていない既存のライブラリがある場合は、それらのバージョン管理をいつでもオンにできます。</span><span class="sxs-lookup"><span data-stu-id="4cd7c-114">If you have existing libraries on your OneDrive for Business site or on your team site that do not have versioning enabled, you can turn versioning on for them at any time.</span></span>


