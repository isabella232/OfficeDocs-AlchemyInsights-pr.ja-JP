---
title: ポリシー catchall
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "3207"
ms.openlocfilehash: 036c171f3c71e60c8c07000b4d0c6ede36bd435c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801671"
---
# <a name="teams-policies"></a><span data-ttu-id="bf771-102">Teams ポリシー</span><span class="sxs-lookup"><span data-stu-id="bf771-102">Teams policies</span></span>

<span data-ttu-id="bf771-103">Microsoft Teams の設定はポリシーによって制御されます。</span><span class="sxs-lookup"><span data-stu-id="bf771-103">Microsoft Teams settings are controlled by policies.</span></span> <span data-ttu-id="bf771-104">変更するには、適切なポリシーを構成し、ユーザーに適用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf771-104">To make a change, you must configure the appropriate policy, and then apply it to users.</span></span> <span data-ttu-id="bf771-105">すべてのユーザーに対してこれを行う最も簡単な方法は、グローバルという名前の既定のポリシーを変更することです。</span><span class="sxs-lookup"><span data-stu-id="bf771-105">The quickest way to do this for all your users is to modify the default policy named Global.</span></span> 

<span data-ttu-id="bf771-106">**注** ポリシーの変更が有効になるには **_最短で 4 時間、最長で 48 時間_** かかります。</span><span class="sxs-lookup"><span data-stu-id="bf771-106">**NOTE** Policy changes take **_at least 4 up to 48 hours to take effect_**.</span></span> <span data-ttu-id="bf771-107">カスタム ポリシーを作成する場合、追加の変更を加えるには少なくとも 4 時間待つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf771-107">If you create a custom policy, you need to wait at least 4 hours before you can make additional changes to it.</span></span> <span data-ttu-id="bf771-108">それからそのポリシーをユーザーに適用することができます。</span><span class="sxs-lookup"><span data-stu-id="bf771-108">Then you can apply that policy to users.</span></span> <span data-ttu-id="bf771-109">つまり、カスタム ポリシーが有効になるまでに、最大 48 時間かかります。</span><span class="sxs-lookup"><span data-stu-id="bf771-109">This means that custom policies can take up to 48 hours to take effect.</span></span> <span data-ttu-id="bf771-110">グローバル ポリシーはすべてのユーザーの既定値として設定されており、その変更が有効になるまで、最大 24 時間かかります。</span><span class="sxs-lookup"><span data-stu-id="bf771-110">Global policies are set as default for all users, and changes to the Global policy can take up to 24 hours to take effect.</span></span> <span data-ttu-id="bf771-111">カスタム ポリシーを作成して、それをユーザーに適用したが、そのポリシーが 48 時間後にも有効になっていない場合、またはグローバル ポリシーを変更して 24 時間以上待っている場合は、サポート ケースを開いてください。</span><span class="sxs-lookup"><span data-stu-id="bf771-111">If you have created a custom policy, applied it to users, and it still hasn't taken effect after 48 hours, or you've modified the Global policy and waited at least 24 hours, please open a support case.</span></span>

<span data-ttu-id="bf771-112">Teams ポリシーは、次の領域に分かれています。</span><span class="sxs-lookup"><span data-stu-id="bf771-112">Teams policies are divided into the following areas:</span></span>

- <span data-ttu-id="bf771-113">[Teams ポリシー](https://docs.microsoft.com/MicrosoftTeams/teams-policies)は、プライベート チャネルの検索と作成においてプライベート チームのユーザー検出を制御します。</span><span class="sxs-lookup"><span data-stu-id="bf771-113">[Teams policies](https://docs.microsoft.com/MicrosoftTeams/teams-policies) control user discovery of private teams in search and creation of private channels.</span></span>  
- <span data-ttu-id="bf771-114">[会議ポリシー](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)は、ロビーの制御など、Teams 会議でユーザーができることを制御します。</span><span class="sxs-lookup"><span data-stu-id="bf771-114">[Meeting policies](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) control what users can do with Teams meetings, including controlling the lobby.</span></span> <span data-ttu-id="bf771-115">全員を許可するように Teams を構成するなど、ロビーの問題に関するヘルプについては、「[ロビーの設定と参加レベルを制御する](https://docs.microsoft.com/alchemyinsights/bypass-lobby)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bf771-115">For help with lobby issues, like configuring Teams to admit everyone, see [Control lobby settings and levels of participation](https://docs.microsoft.com/alchemyinsights/bypass-lobby).</span></span>
- <span data-ttu-id="bf771-116">[メッセージング ポリシー](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)は、チャットのオンとオフの切り替え、チャットの削除、開封確認の要求、giphy とステッカーの使用など、ユーザーがチャットとメッセージでできることを制御します。</span><span class="sxs-lookup"><span data-stu-id="bf771-116">[Messaging policies](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) control what users can do with chat and messages, including turning chat on or off, deleting chats, requesting read receipts, using giphys and stickers, and more.</span></span>
- <span data-ttu-id="bf771-117">[アプリ セットアップ ポリシー](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies)は、カスタム アプリやサード パーティ アプリなど、ユーザーが利用できるアプリと、表​​示される順序を制御します。</span><span class="sxs-lookup"><span data-stu-id="bf771-117">[App setup policies](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) control which apps are available to users, including custom and third-party apps, and the order in which they appear.</span></span>  
- <span data-ttu-id="bf771-118">Teams のデータ[保持ポリシー](https://docs.microsoft.com/microsoftteams/retention-policies)は、Microsoft 365 のセキュリティ/コンプライアンス センターで確認できます。</span><span class="sxs-lookup"><span data-stu-id="bf771-118">Data [retention policies](https://docs.microsoft.com/microsoftteams/retention-policies) for Teams are found in the Microsoft 365 security and Compliance Center.</span></span>
- <span data-ttu-id="bf771-119">Teams のアドレス帳ポリシーは、[スコープが設定されたディレクトリの検索](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search)によって設定されます。</span><span class="sxs-lookup"><span data-stu-id="bf771-119">Teams address book policies are set via [scoped directory search](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search).</span></span>