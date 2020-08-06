---
title: Intune でメール プロファイルを使用する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "46556221"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="c9c67-102">Intune でメール プロファイルを使用する</span><span class="sxs-lookup"><span data-stu-id="c9c67-102">Using email profiles with Intune</span></span>

<span data-ttu-id="c9c67-103">Intune を使用すると、複数のデバイス プラットフォームでネイティブ (組み込み) のメール クライアントのメール プロファイルを作成して展開することができます。</span><span class="sxs-lookup"><span data-stu-id="c9c67-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="c9c67-104">既存のプロファイルの存在の処理方法やメール プロファイルを削除する方法など、メール プロファイルに関するいくつかの制限事項の詳細については、「[Add email settings to devices using Intune (Intune を使用してメール設定をデバイスに追加する)](https://docs.microsoft.com/intune/email-settings-configure)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9c67-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="c9c67-105">各デバイス プラットフォーム用にメール プロファイルを作成する方法の詳細については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9c67-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="c9c67-106">Android device settings to configure email, authentication, and synchronization in Intune (Intune でメール、認証、同期を構成するための Android デバイスの設定)</span><span class="sxs-lookup"><span data-stu-id="c9c67-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="c9c67-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune (Microsoft Intune で iOS デバイスおよび iPadOS デバイス用のメール設定を追加する)</span><span class="sxs-lookup"><span data-stu-id="c9c67-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="c9c67-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1 (Microsoft Intune での、Windows Phone 8.1 を実行するデバイス用のメール プロファイル設定)</span><span class="sxs-lookup"><span data-stu-id="c9c67-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="c9c67-109">Email profile settings for devices running Windows 10 in Microsoft Intune (Microsoft Intune での、Windows 10 を実行するデバイス用のメール プロファイル設定)</span><span class="sxs-lookup"><span data-stu-id="c9c67-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="c9c67-110">**同期に関する一般的な問題**</span><span class="sxs-lookup"><span data-stu-id="c9c67-110">**Common syncing issue**</span></span>

<span data-ttu-id="c9c67-111">**Android メール プロファイルの KNOX があるために、ユーザーの連絡先、カレンダー、タスクがユーザーのデバイスに同期されない。**</span><span class="sxs-lookup"><span data-stu-id="c9c67-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="c9c67-112">Android KNOX メール プロファイルの KNOX では、デバイスに同期するコンテンツ タイプを管理者が決定することができ、同期する場合はそれぞれのタイプを有効に設定します。</span><span class="sxs-lookup"><span data-stu-id="c9c67-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="c9c67-113">[**Not configured (未構成)**] (既定) に設定されているコンテンツ タイプは、自動的には同期されません。</span><span class="sxs-lookup"><span data-stu-id="c9c67-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="c9c67-114">ユーザーは、希望するコンテンツ タイプをデバイス上で直接手動で有効にできますが、その構成は Intune ポリシーの設定により上書きされ、そのコンテンツ タイプの同期は停止されます。</span><span class="sxs-lookup"><span data-stu-id="c9c67-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

