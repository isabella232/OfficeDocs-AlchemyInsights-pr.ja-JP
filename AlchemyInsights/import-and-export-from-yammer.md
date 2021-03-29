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
# <a name="import-and-export-from-yammer"></a>Yammer からのインポートとエクスポート

**インポート**

ユーザーインポートのオプションは、使用している Yammer ネットワークが [Microsoft 365 ネイティブ モード](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)であるかどうかによって異なります。

- **非ネイティブ モード**: グループ設定内の、[[アドレス帳から追加](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294)] (最大 100 ユーザーまで) を使用してユーザーをグループにインポートするか、またはネットワーク管理者内の [[一括更新](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)] を使用して、ユーザーをネットワークにインポートすることができます。
- **ネイティブ モード**: グループ メンバーシップとネットワーク メンバーシップの操作は、[Microsoft 365 管理ポータル](https://docs.microsoft.com/microsoft-365/admin/add-users)、[Azure AD ポータル](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)、または別の Azure AD オプションを使用して実行する必要があります。 ネイティブ モードのネットワークでは、一括更新やその他のレガシ機能にアクセスできません。

> [!IMPORTANT]
> データ エクスポート機能が別のネットワークで使用されている場合でも、Yammer は ネットワーク管理者内からのコンテンツのインポートをサポートしていませんでした。 コンテンツは、パートナー ソリューションまたは Yammer REST API で再投稿することができます。

**エクスポート**

[ネットワーク管理者内のネットワーク データのエクスポート](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data)では、メッセージやファイルを含む Yammer ネットワークからのコンテンツのエクスポートを許可することができます。 添付ファイルは非常に大きく、エクスポートの完了までに時間が長くかかる場合があります。 アクティブなネットワークは、[データ エクスポート API](https://developer.yammer.com/docs/data-export-api) を使用して、日ごとにまたは週ごとにエクスポートすることをお勧めします。 Microsoft サポートでは、この目的のためのカスタム スクリプトを提供していません。

個々のユーザーのコンテンツをエクスポートするために、[GDPR エクスポート](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise)が別個に存在します。