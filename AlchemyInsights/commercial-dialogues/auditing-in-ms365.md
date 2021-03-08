---
title: Microsoft 365 での監査
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484120"
---
# <a name="auditing-in-microsoft-365"></a>Microsoft 365 での監査

Microsoft 365 での監査について知っておくべきことがいくつかあります。

1. Exchange 管理者のアクティビティは、既定で監査されます。
1. 現在、すべてのユーザーに対してメールボックス監査を既定でオンにしています。 詳細については、[こちら](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)をクリックしてください。 それまでは、1 人または組織全体で手動で有効にする手順が必要な場合は、下の [メールボックスの監査を有効にする] ボタンを選択してください。
1. Microsoft 365 グループ メールボックスとパブリック フォルダー メールボックスは、監査ログをサポートしていません。
1. SharePoint および OneDrive の場合、監査を有効にするために追加の構成は必要ありません。 監査されるアクティビティについては、以下を参照してください。
    1. [ファイル アクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [フォルダー アクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [共有アクティビティとアクセス アクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)。
1. サービスごとのすべての監査済みアクティビティのリストについては、「[監査済みアクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)」を参照してください。
