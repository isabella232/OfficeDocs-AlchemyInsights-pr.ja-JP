---
title: Teams のファイルへのアクセス
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2675"
- "9000710"
ms.openlocfilehash: 8731cad13ad5bacb7f69b70c91d50524ce38d558
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/30/2019
ms.locfileid: "40923562"
---
# <a name="accessing-files-in-microsoft-teams"></a><span data-ttu-id="e7f4b-102">Microsoft Teams のファイルへのアクセス</span><span class="sxs-lookup"><span data-stu-id="e7f4b-102">Accessing files in Microsoft Teams</span></span>

<span data-ttu-id="e7f4b-103">ユーザーが Microsoft Teams のファイルにアクセスするのが困難な場合は、まず、ファイルがプライベートチャットまたはチャネル会話に添付されているかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-103">If users have difficulty accessing a file in Microsoft Teams, first determine whether the file is attached to a private chat or a channel conversation.</span></span> <span data-ttu-id="e7f4b-104">チーム チャンネルは、チームの全員があけすけに会話できる場所です。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-104">Team channels are places where everyone on the team can openly have conversations.</span></span> <span data-ttu-id="e7f4b-105">プライベートチャットはチャット内のユーザーにのみ表示されます (また、チャットで共有するファイルは OneDrive for Business に保存されます)。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-105">Private chats are only visible to those people in the chat (and files that you share in a chat are stored in OneDrive for Business).</span></span>

<span data-ttu-id="e7f4b-106">ユーザーがプライベートチャットでファイルを共有する場合、ファイルは共有ユーザーの OneDrive for Business に保存されます。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-106">When users share files in private chats, the file is stored on the sharing user's OneDrive for Business.</span></span> <span data-ttu-id="e7f4b-107">ユーザーが既存のプライベートチャットに追加された場合、元の所有者がファイルを再度共有しない限り、ファイルにアクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-107">If a user was added to an existing private chat, they won't be able to access the files unless the original owner re-shares the file.</span></span>    

<span data-ttu-id="e7f4b-108">**チャネル会話の場合:**</span><span class="sxs-lookup"><span data-stu-id="e7f4b-108">**For channel conversations:**</span></span>

- <span data-ttu-id="e7f4b-109">[Microsoft Teams でのファイルの共有](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams)は、SharePoint または OneDrive で構成された設定に基づいています。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-109">[Sharing files in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) is based on the settings configured in SharePoint or OneDrive.</span></span> 
- <span data-ttu-id="e7f4b-110">Teams でのファイルの共有と共同作業の方法の詳細については[、「チームでファイルの共同作業](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-110">Review [Collaborate on files with your Team](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) to learn more about how Teams allows your organization to share and collaborate on files.</span></span> 
- <span data-ttu-id="e7f4b-111">新しいチームメンバーがファイルへのアクセスに遅延を感じる場合は、サポートチケットを開いてレプリケーションが完了するまで、少なくとも**4 時間**待つようにしてください。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-111">If new team members experience a delay in accessing files, please wait at least **4 hours** before opening a support ticket to allow replication to complete.</span></span> 

<span data-ttu-id="e7f4b-112">ユーザーがチームチャネルの [ファイル] タブを使用してファイルにアクセスでき、"これらのファイルは使用できません" というエラーが表示される場合は、SharePoint サイトまたはドキュメントライブラリの名前が変更されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-112">If users could previously access files via the Files tab on a team channel, and you get a "these files are no longer available" error, check to see if the SharePoint site or document library has been renamed.</span></span> <span data-ttu-id="e7f4b-113">Teams の SharePoint サイトとドキュメントライブラリの名前を変更することはまだサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-113">Renaming SharePoint sites and document libraries for Teams is not yet supported.</span></span> <span data-ttu-id="e7f4b-114">この問題を解決するには、このチームに使用されているチームサイトを開き、ライブラリの名前を "Shared Documents" に戻します。</span><span class="sxs-lookup"><span data-stu-id="e7f4b-114">To resolve this issue, open the team site used for this team and rename the library back to “Shared Documents”.</span></span>