---
title: Android デバイスを Intune に登録する
ms.author: erikje
author: erikje
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000652"
- "2494"
ms.openlocfilehash: c39fec48f791d5cc4a97688cc7b5cd93010403a2
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791263"
---
# <a name="enrolling-android-devices-into-intune"></a><span data-ttu-id="7aa80-102">Android デバイスを Intune に登録する</span><span class="sxs-lookup"><span data-stu-id="7aa80-102">Enrolling Android devices into Intune</span></span>

<span data-ttu-id="7aa80-103">Android デバイスの管理者登録から Android Enterprise にユーザーを移行する場合は、次のことを確認してください。[ Android デバイスを管理者から 、作業プロファイル管理に移動](https://docs.microsoft.com/mem/intune/enrollment/android-move-device-admin-work-profile)。</span><span class="sxs-lookup"><span data-stu-id="7aa80-103">If you are looking to migrate users from Android Device Administrator enrollment to Android Enterprise, please review: [Move Android devices from device administrator to work profile management](https://docs.microsoft.com/mem/intune/enrollment/android-move-device-admin-work-profile).</span></span>

<span data-ttu-id="7aa80-104">Intune は、次の Android デバイスの登録をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="7aa80-104">Intune supports the enrollment of the following Android devices:</span></span>  

- [<span data-ttu-id="7aa80-105">Samsung Knox, Zebra, Device 管理者</span><span class="sxs-lookup"><span data-stu-id="7aa80-105">Samsung Knox, Zebra, Device Administrator</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-enroll-device-administrator)
- [<span data-ttu-id="7aa80-106">Android Enterprise の作業プロフィール</span><span class="sxs-lookup"><span data-stu-id="7aa80-106">Android Enterprise work profile</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-enterprise-overview)
- [<span data-ttu-id="7aa80-107">Android Enterprise 専用</span><span class="sxs-lookup"><span data-stu-id="7aa80-107">Android Enterprise dedicated</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-dedicated-devices-fully-managed-enroll)
- [<span data-ttu-id="7aa80-108">完全に管理されている Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="7aa80-108">Android Enterprise fully managed</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-fully-managed-enroll)

<span data-ttu-id="7aa80-109">Android デバイスの登録をセットアップする前に、[[前提条件を確認してください](https://docs.microsoft.com/intune/enrollment/android-enroll)]。</span><span class="sxs-lookup"><span data-stu-id="7aa80-109">Before setting up enrollment for Android devices, [review the pre-requisites](https://docs.microsoft.com/intune/enrollment/android-enroll).</span></span>  

<span data-ttu-id="7aa80-110">デバイス登録のトラブルシューティング全般および Android 登録のエラーについては、「[Microsoft Intune でデバイス登録のトラブルシューティングを行う](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-android-enrollment)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7aa80-110">For information on troubleshooting device enrollment in general and some Android enrollment errors, see [Troubleshoot device enrollment in Microsoft Intune](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-android-enrollment).</span></span>

<span data-ttu-id="7aa80-111">ユーザーに発生している登録に関する問題は、Intune のトラブルシューティング ブレードに関する説明を使用して特定することもできます。</span><span class="sxs-lookup"><span data-stu-id="7aa80-111">You can also use the content describing the Intune Troubleshooting blade to help identify what enrolment issues your users are experiencing.</span></span>
