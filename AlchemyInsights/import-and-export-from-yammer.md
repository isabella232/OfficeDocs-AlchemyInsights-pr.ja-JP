---
title: Yammer からのインポートとエクスポート
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038276"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="b93ca-102">Yammer からのインポートとエクスポート</span><span class="sxs-lookup"><span data-stu-id="b93ca-102">Import and export from Yammer</span></span>

<span data-ttu-id="b93ca-103">**インポート**</span><span class="sxs-lookup"><span data-stu-id="b93ca-103">**Import**</span></span>

<span data-ttu-id="b93ca-104">ユーザーインポートのオプションは、使用している Yammer ネットワークが [Microsoft 365 ネイティブ モード](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)であるかどうかによって異なります。</span><span class="sxs-lookup"><span data-stu-id="b93ca-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="b93ca-105">**非ネイティブ モード**: グループ設定内の、[[アドレス帳から追加](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294)] (最大 100 ユーザーまで) を使用してユーザーをグループにインポートするか、またはネットワーク管理者内の [[一括更新](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)] を使用して、ユーザーをネットワークにインポートすることができます。</span><span class="sxs-lookup"><span data-stu-id="b93ca-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="b93ca-106">**ネイティブ モード**: グループ メンバーシップとネットワーク メンバーシップの操作は、[Microsoft 365 管理ポータル](https://docs.microsoft.com/microsoft-365/admin/add-users)、[Azure AD ポータル](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)、または別の Azure AD オプションを使用して実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b93ca-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="b93ca-107">ネイティブ モードのネットワークでは、一括更新やその他のレガシ機能にアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="b93ca-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b93ca-108">データ エクスポート機能が別のネットワークで使用されている場合でも、Yammer は ネットワーク管理者内からのコンテンツのインポートをサポートしていませんでした。</span><span class="sxs-lookup"><span data-stu-id="b93ca-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="b93ca-109">コンテンツは、パートナー ソリューションまたは Yammer REST API で再投稿することができます。</span><span class="sxs-lookup"><span data-stu-id="b93ca-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="b93ca-110">**エクスポート**</span><span class="sxs-lookup"><span data-stu-id="b93ca-110">**Export**</span></span>

<span data-ttu-id="b93ca-111">[ネットワーク管理者内のネットワーク データのエクスポート](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data)では、メッセージやファイルを含む Yammer ネットワークからのコンテンツのエクスポートを許可することができます。</span><span class="sxs-lookup"><span data-stu-id="b93ca-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="b93ca-112">添付ファイルは非常に大きく、エクスポートの完了までに時間が長くかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="b93ca-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="b93ca-113">アクティブなネットワークは、[データ エクスポート API](https://developer.yammer.com/docs/data-export-api) を使用して、日ごとにまたは週ごとにエクスポートすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b93ca-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="b93ca-114">Microsoft サポートでは、この目的のためのカスタム スクリプトを提供していません。</span><span class="sxs-lookup"><span data-stu-id="b93ca-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="b93ca-115">個々のユーザーのコンテンツをエクスポートするために、[GDPR エクスポート](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise)が別個に存在します。</span><span class="sxs-lookup"><span data-stu-id="b93ca-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>