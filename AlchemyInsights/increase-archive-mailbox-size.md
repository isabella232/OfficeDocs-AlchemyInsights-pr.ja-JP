---
title: 305 アーカイブ メールボックスのサイズを増やす
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 28086145d8769bd06ef6352257a820146c5f237d
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36397245"
---
# <a name="increase-the-archive-mailbox-size"></a>アーカイブ メールボックスの容量を増やす

Office 365 では、ユーザー アカウントに割り当てられているライセンスに基づいて、アーカイブ メールボックスのサイズが[制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)されます。 アーカイブ メールボックスが許可されているサイズの 90% に達すると、ユーザーはメール通知を受け取ります。 アーカイブ メールボックスがサイズの上限に達すると、ユーザーは追加のアイテムをアーカイブ メールボックスに移動することができなくなります。 アーカイブ メールボックスがサイズの上限に達しても、Office 365 によりサイズが拡張されることはありません。 ユーザーは、次の操作を実行するとアーカイブ メールボックスの領域を開放することができます。

- Outlook を使用してアイテムを .pst ファイルにエクスポートする

- アーカイブ メールボックスからアイテムを削除します。

Office 365 では、Office 365 Enterprise E3 および E5 のライセンスで**無制限アーカイブ**が提供されています。 管理者は、アーカイブ メールボックスのサイズが最大サイズに達する前にこの機能を有効にする必要があります。 無制限アーカイブが有効になっている場合、アーカイブ メールボックスに空き領域が追加されるまで最大で 30 日かかります。 このため、サイズが拡大される間もユーザーがアーカイブ メールボックスを使用し続けることができるよう、管理者はアーカイブ メールボックスの空き領域を確認することをお勧めします。 詳細については、「[Office 365 での無制限アーカイブの概要](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving)」と「[Office 365 で無制限アーカイブを有効にする](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)」を参照してください。

Outlook からアーカイブ メールボックスにアクセスする方法の詳細については、「[自動拡張アーカイブ内のアイテムにアクセスするための Outlook の要件](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)」を参照してください。 アイテムをアーカイブ メールボックスに自動的に移動するアイテム保持ポリシーを構成する方法については、「[Office 365 組織のメールボックスのアーカイブおよび削除ポリシーを設定する](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)」を参照してください。

**注**: 自動拡張アーカイブは、Exchange 2010 のプライマリ メールボックスではサポートされていません。
