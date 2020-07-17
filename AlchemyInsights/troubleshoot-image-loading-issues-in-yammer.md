---
title: Yammer での画像の読み込みに関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148476"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="8217a-102">Yammer での画像の読み込みに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="8217a-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="8217a-103">Yammerの写真とファイルのプレビューで問題が発生した場合は、問題がすべてのユーザーに発生するかどうか、モバイルデバイスで発生するかどうか、および添付ファイルをアップロードする時に再現できるかを確認してトラブルシューティングします。</span><span class="sxs-lookup"><span data-stu-id="8217a-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="8217a-104">**プロフィール写真の問題**</span><span class="sxs-lookup"><span data-stu-id="8217a-104">**Profile photo issues**</span></span>  

<span data-ttu-id="8217a-105">エンドユーザーが Microsoft 365 経由で Yammer にサインインする場合、プロフィール写真を含むプロファイルを変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8217a-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="8217a-106">ユーザーがプロファイルの更新を許可していない場合、管理者がユーザーの代わりに更新を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="8217a-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="8217a-107">詳細については、「[Office Delve でプロファイルを表示して更新する](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8217a-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="8217a-108">プロファイル写真などのプロファイル編集の詳細については、[ Yammerプロファイルの変更と設定 ](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8217a-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="8217a-109">更新されたプロファイルの写真は、プロファイルの属性とは違う方法で同期されます。</span><span class="sxs-lookup"><span data-stu-id="8217a-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="8217a-110">ユーザーは、自分のプロファイル写真を同期するためにサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8217a-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="8217a-111">詳しくは、[ユーザー プロファイルの画像は Office 365 から Yammer に更新されますか ?](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8217a-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="8217a-112">Yammer のユーザーライフサイクルの詳細については、[Yammer ユーザーをライフサイクルを通じて Office 365 から管理する](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8217a-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="8217a-113">Microsoft 365 のプロファイル画像同期の詳細については、[「Microsoft 365のプロファイル画像の同期」](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8217a-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="8217a-114">**ドキュメントのプレビューとサムネイル画像の問題**</span><span class="sxs-lookup"><span data-stu-id="8217a-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="8217a-115">ファイルまたは画像が Yammer に投稿されると、プレビューが表示されない理由は次のとおりです:</span><span class="sxs-lookup"><span data-stu-id="8217a-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="8217a-116">ファイルが破損しているため処理することができません。</span><span class="sxs-lookup"><span data-stu-id="8217a-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="8217a-117">ファイルがまだ SharePoint Online にアップロードされていない、または Yammer がその他の理由で無効なメタデータを持っています。</span><span class="sxs-lookup"><span data-stu-id="8217a-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="8217a-118">プレビューイメージの読み込みに必要な URL はブロックされます。</span><span class="sxs-lookup"><span data-stu-id="8217a-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="8217a-119">ユーザーが投稿前にファイルプレビューを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8217a-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="8217a-120">サービスの問題により、プレビューが生成されませんでした。</span><span class="sxs-lookup"><span data-stu-id="8217a-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="8217a-121">**注** プレビューのリンクとファイルのアップロードは異なる動作をする場合があります。</span><span class="sxs-lookup"><span data-stu-id="8217a-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="8217a-122">インターネット上のファイルへのリンクまたは追加の認証が必要なリンクは、正しく表示されない場合があります。</span><span class="sxs-lookup"><span data-stu-id="8217a-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="8217a-123">詳しくは、[「Yammer メッセージにファイルまたは画像を添付する」](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8217a-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 