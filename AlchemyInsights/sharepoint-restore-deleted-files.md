---
title: 削除したファイルまたはフォルダーの復元
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 1672f425719597b93b8ef05865797714c3b19e42
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35085897"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="262a4-102">削除したファイルまたはフォルダーの復元</span><span class="sxs-lookup"><span data-stu-id="262a4-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="262a4-103">SharePoint Online では、実際の削除から 14 日間、すべてのコンテンツがバックアップされます。</span><span class="sxs-lookup"><span data-stu-id="262a4-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="262a4-104">[ごみ箱] または [ファイルの復元] からコンテンツを復元できない場合、管理者は Microsoft サポートに連絡して 14 日間の期間内に復元を要求できます。</span><span class="sxs-lookup"><span data-stu-id="262a4-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="262a4-105">バックアップからの復元は、サイト コレクションまたはサブサイトに対してのみ実行可能です。特定のファイル、リスト、またはライブラリの復元はできません。</span><span class="sxs-lookup"><span data-stu-id="262a4-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="262a4-106">SharePoint からアイテムまたはサイトを削除した時点で、それらがすぐに消去されることはありません。</span><span class="sxs-lookup"><span data-stu-id="262a4-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="262a4-107">削除したアイテムは、一定の期間 [ごみ箱] に移動されます。</span><span class="sxs-lookup"><span data-stu-id="262a4-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="262a4-108">その間は、削除したアイテムを元の場所に復元できます。</span><span class="sxs-lookup"><span data-stu-id="262a4-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="262a4-109">詳細については、次のリンク先を参照してください。</span><span class="sxs-lookup"><span data-stu-id="262a4-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="262a4-110">[SharePoint サイトのごみ箱のアイテムを復元する](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US)</span><span class="sxs-lookup"><span data-stu-id="262a4-110">Restore items in the Recycle Bin of a SharePoint site</span></span>

[<span data-ttu-id="262a4-111">OneDrive で削除したファイルまたはフォルダーを復元する</span><span class="sxs-lookup"><span data-stu-id="262a4-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="262a4-112">削除されたサイト コレクションを復元する (グループやコミュニケーションなどのサイトを含む)</span><span class="sxs-lookup"><span data-stu-id="262a4-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="262a4-113">削除された OneDrive を復元する</span><span class="sxs-lookup"><span data-stu-id="262a4-113">Restore a deleted OneDrive</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="262a4-114">ごみ箱の一括操作について、管理者は [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) の使用について検討してください。</span><span class="sxs-lookup"><span data-stu-id="262a4-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="262a4-115">**ファイルの復元機能**</span><span class="sxs-lookup"><span data-stu-id="262a4-115">**Utilize the OneDrive Files Restore feature**.</span></span>

<span data-ttu-id="262a4-116">OneDrive または SharePoint の多数のファイルを削除、上書き、破損した場合や多数のファイルがマルウェアに感染した場合には、ファイルの復元機能を使用して、OneDrive または SharePoint のライブラリ全体を以前の状態に復元できます。</span><span class="sxs-lookup"><span data-stu-id="262a4-116">If lots of your OneDrive files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive to a previous time using the OneDrive Files restore feature.</span></span>

[<span data-ttu-id="262a4-117">OneDrive ライブラリを復元する</span><span class="sxs-lookup"><span data-stu-id="262a4-117">Restore a deleted OneDrive</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="262a4-118">ドキュメント ライブラリを復元する</span><span class="sxs-lookup"><span data-stu-id="262a4-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

