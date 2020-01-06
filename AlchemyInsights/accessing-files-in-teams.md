---
title: Teams 内のファイルへアクセスする
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/30/2019
ms.locfileid: "40923562"
---
# <a name="accessing-files-in-microsoft-teams"></a><span data-ttu-id="68842-102">Microsoft Teams 内のファイルへアクセスする</span><span class="sxs-lookup"><span data-stu-id="68842-102">Secure files in Microsoft Teams</span></span>

<span data-ttu-id="68842-103">ユーザが Microsoft Teams のファイルにアクセスできない場合は、まずそのファイルがプライベート チャットまたはチャネルの会話に添付されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="68842-103">If users have difficulty accessing a file in Microsoft Teams, first determine whether the file is attached to a private chat or a channel conversation.</span></span> <span data-ttu-id="68842-104">チーム チャネルは、チームの全員が率直に会話できる場所です。</span><span class="sxs-lookup"><span data-stu-id="68842-104">Team channels are places where everyone on the team can openly have conversations.</span></span> <span data-ttu-id="68842-105">プライベート チャットは、チャットの参加者にのみ表示されます (チャットで共有するファイルは OneDrive for Business に保存されます)。</span><span class="sxs-lookup"><span data-stu-id="68842-105">Private chats are only visible to those people in the chat (and files that you share in a chat are stored in OneDrive for Business).</span></span>

<span data-ttu-id="68842-106">ユーザーがプライベート チャットでファイルを共有する場合、ファイルは共有ユーザーの OneDrive for Business に保存されます。</span><span class="sxs-lookup"><span data-stu-id="68842-106">When users share files in private chats, the file is stored on the sharing user's OneDrive for Business.</span></span> <span data-ttu-id="68842-107">ユーザーが既存のプライベート チャットに追加された場合、元の所有者がそのファイルを再共有しない限り、ファイルにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="68842-107">If a user was added to an existing private chat, they won't be able to access the files unless the original owner re-shares the file.</span></span>    

<span data-ttu-id="68842-108">**チャネル会話の場合:**</span><span class="sxs-lookup"><span data-stu-id="68842-108">**For channel conversations:**</span></span>

- <span data-ttu-id="68842-109">[Microsoft Teams でのファイルの共有](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams)は、SharePoint または OneDrive で構成された設定に基づいて行われます。</span><span class="sxs-lookup"><span data-stu-id="68842-109">[Sharing files in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) is based on the settings configured in SharePoint or OneDrive.</span></span> 
- <span data-ttu-id="68842-110">Teams でファイルを共有して共同作業できるようにする方法については、「[自分のチームでファイルでの共同作業を行う](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="68842-110">Review [Collaborate on files with your Team](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) to learn more about how Teams allows your organization to share and collaborate on files.</span></span> 
- <span data-ttu-id="68842-111">新しいチーム メンバーがファイルへアクセスする際に遅延が発生した場合は、少なくとも **4 時間**待ってから、サポート チケットを開いてレプリケーションを完了してください。</span><span class="sxs-lookup"><span data-stu-id="68842-111">If new team members experience a delay in accessing files, please wait at least **4 hours** before opening a support ticket to allow replication to complete.</span></span> 

<span data-ttu-id="68842-112">以前にはユーザーがチーム チャネルの [ファイル] タブからファイルにアクセスでき、「これらのファイルは利用できなくなりました」というエラーが表示される場合は、SharePoint サイトまたはドキュメント ライブラリの名前が変更されているかどうかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="68842-112">If users could previously access files via the Files tab on a team channel, and you get a "these files are no longer available" error, check to see if the SharePoint site or document library has been renamed.</span></span> <span data-ttu-id="68842-113">Teams の SharePoint サイトとドキュメント ライブラリの名前の変更は、まだサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68842-113">Renaming SharePoint sites and document libraries for Teams is not yet supported.</span></span> <span data-ttu-id="68842-114">この問題を解決するには、このチームに使用されているチーム サイトを開いて、ライブラリの名前を [共有ドキュメント] に戻します。</span><span class="sxs-lookup"><span data-stu-id="68842-114">To resolve this issue, open the team site used for this team and rename the library back to “Shared Documents”.</span></span>