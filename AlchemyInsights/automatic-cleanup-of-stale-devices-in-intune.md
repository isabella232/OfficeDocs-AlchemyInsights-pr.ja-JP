---
title: Intune での古いデバイスの自動クリーンアップ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715026"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="382fd-102">Intune での古いデバイスの自動クリーンアップ</span><span class="sxs-lookup"><span data-stu-id="382fd-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="382fd-103">Intune では、管理者が 90 日から 270 日の間で期間を設定し、この期間を過ぎた場合に古いデバイスがサービスから削除されるように構成できます。</span><span class="sxs-lookup"><span data-stu-id="382fd-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="382fd-104">この設定は組織全体に適用され、アクティブになると直ちに有効になります。</span><span class="sxs-lookup"><span data-stu-id="382fd-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="382fd-105">設定された期間を超える期間に渡って Intune サーバーにチェックインされなかったデバイスは、完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="382fd-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="382fd-106">**注** このクリーンアップ アクションの対象にできるのは、MDM デバイス オブジェクトのみです。</span><span class="sxs-lookup"><span data-stu-id="382fd-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="382fd-107">EAS のみのデバイス オブジェクトは除外されます。</span><span class="sxs-lookup"><span data-stu-id="382fd-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="382fd-108">デバイスがデバイスのクリーンアップ設定とその "状態" に基づくデバイス削除の対象になるタイミングの詳細については、次の設定を確認してください。</span><span class="sxs-lookup"><span data-stu-id="382fd-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="382fd-109">Setting (設定): **Delete devices after last check-in date (最終チェックイン日の後にデバイスを削除する): Yes (日数の値 (N) が指定されています)**</span><span class="sxs-lookup"><span data-stu-id="382fd-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="382fd-110">デバイスによる最後の正常なチェックインから指定されている日数が経過すると、Intune サービスは設定で構成されている (N) の値を使用してデバイスを削除します。</span><span class="sxs-lookup"><span data-stu-id="382fd-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="382fd-111">Setting (設定):  **Delete devices after last check-in date (最終チェックイン日の後にデバイスを削除する): No**</span><span class="sxs-lookup"><span data-stu-id="382fd-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="382fd-112">デバイスの証明書の有効期限が切れてから 180 日経過し、証明書が更新されない場合は、デバイスは削除されます。</span><span class="sxs-lookup"><span data-stu-id="382fd-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="382fd-113">**注** いずれの場合も、Intune にデバイスが正常に登録されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="382fd-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="382fd-114">登録は、デバイスを初めて Intune サービスにチェックインする際に実行されます。</span><span class="sxs-lookup"><span data-stu-id="382fd-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="382fd-115">デバイスが Intune に正常に登録されたにもかかわらず Intune 登録済みとなっていない場合、このデバイスは登録から 270 日後に削除されます。</span><span class="sxs-lookup"><span data-stu-id="382fd-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="382fd-116">(デバイスは 90 日後に取消済みとマークされ、それからさらに 180 日後に記録が削除されます。)</span><span class="sxs-lookup"><span data-stu-id="382fd-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="382fd-117">Intune コンソールには現在、特定のデバイスのデバイス証明書の有効期限を設定するための機能が備わっていません。</span><span class="sxs-lookup"><span data-stu-id="382fd-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>