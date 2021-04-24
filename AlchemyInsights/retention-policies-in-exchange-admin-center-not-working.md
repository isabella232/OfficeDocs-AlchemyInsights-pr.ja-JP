---
title: Exchange 管理センターでアイテム保持ポリシーが動作しない
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952233"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 管理センターでのアイテム保持ポリシー

下記の設定の自動チェックを実行する場合は、このページの上部にある [戻る <--] ボタンを選択し、メールをアーカイブメールボックスに移動できないユーザーのメールアドレスを入力します。

Exchange 管理センターのアイテム保持ポリシーがメールボックスに適用されない、またはアイテムがアーカイブ メールボックスに移動しないという問題がある場合は、以下を確認してください。

**根本原因:**

- **管理フォルダー用アシスタント** はユーザーのメールボックスを処理していません。 管理フォルダー用アシスタントは、7 日に一度クラウドベース組織のすべてのメールボックスを処理しようとします。

  **解決策:** 管理フォルダー用アシスタントを実行します。

- メールボックスで **RetentionHold** が **有効** になっています。 メールボックスが RetentionHold に配置されている場合、その間、メールボックスのアイテム保持ポリシーは処理されません。

  **解決策:** 保持ホールド設定の状態を確認し、必要に応じて更新します。 詳細については、「[メールボックスのアイテム保持ホールド](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)」を参照してください。
 
**注:** メールボックス サイズが 10 MB 未満の場合、管理フォルダー用アシスタントによってメールボックスは自動処理されません。
 
Exchange 管理センターのアイテム保持ポリシーの詳細については、以下を参照してください。

- [保持タグおよびアイテム保持ポリシー](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [メールボックスにアイテム保持ポリシーを適用する](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)か、[アイテム保持タグを追加または削除する](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [メールボックスに適用されている保留の種類を特定する方法](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
