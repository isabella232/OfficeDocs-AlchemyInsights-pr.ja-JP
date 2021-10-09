---
title: 305 アーカイブ メールボックスのサイズを増やす
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "305"
- "7494"
- "3100006"
ms.assetid: ''
ms.openlocfilehash: d74a1baa02a74c8efd3be75ed711a2e994b9b552
ms.sourcegitcommit: 68b50235d10ebb92b594ac3224c55cf0e8452ac9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/07/2021
ms.locfileid: "60226097"
---
# <a name="increase-the-archive-mailbox-size"></a>アーカイブ メールボックスの容量を増やす

Microsoft 365 では、ユーザー アカウントに割り当てられているライセンスに基づいて、アーカイブ メールボックスのサイズが制限されます。 アーカイブ メールボックスが許可されたサイズの 90% に達すると、ユーザーはメール通知を受け取ります。

アーカイブ メールボックスがサイズの上限に達すると、ユーザーは追加のアイテムをアーカイブ メールボックスに移動することができなくなります。 アーカイブ メールボックスがサイズの上限に達しても、Microsoft 365 によりサイズが拡張されることはありません。 代わりに、ユーザーは次の操作を実行するとアーカイブ メールボックスの領域を開放することができます。

- Outlook を使用してアイテムを .pst ファイルにエクスポートします。
- アーカイブ メールボックスからアイテムを削除します。

ただし、Microsoft 365 は、Office 365 Enterprise E3 および E5 ライセンスの自動拡張アーカイブを提供します。 これは、アーカイブ メールボックスが最大サイズに達する前に有効にする必要があります。 自動拡張アーカイブが有効になっている場合、アーカイブ メールボックスに空き領域が追加されるまで最大で 30 日かかります。

詳細については、「[自動拡張アーカイブの概要](https://docs.microsoft.com/microsoft-365/compliance/autoexpanding-archiving)」および「[自動拡張アーカイブを有効にする - 管理者ヘルプ](https://docs.microsoft.com/microsoft-365/compliance/enable-autoexpanding-archiving)」を参照してください。

Outlook を使用してアーカイブにアクセスする方法については、「[自動拡張アーカイブ内のアイテムにアクセスするための Outlook の要件](https://docs.microsoft.com/microsoft-365/compliance/autoexpanding-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)」を参照してください。

アイテムをアーカイブ メールボックスに自動的に移動するアイテム保持ポリシーの構成については、「[Microsoft 365 組織のメールボックスのアーカイブと削除ポリシーを設定する](https://docs.microsoft.com//microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)」を参照してください。