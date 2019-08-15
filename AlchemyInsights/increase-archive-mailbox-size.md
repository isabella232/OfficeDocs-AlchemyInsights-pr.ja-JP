---
title: 305アーカイブメールボックスのサイズを増やす
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36397245"
---
# <a name="increase-the-archive-mailbox-size"></a>アーカイブメールボックスのサイズを増やす

Office 365 では、ユーザーアカウントに割り当てられているライセンスに基づいて、アーカイブメールボックスのサイズが[制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)されます。 アーカイブメールボックスが許可されたサイズの 90% に達すると、ユーザーはメール通知を受信します。 アーカイブメールボックスのサイズが制限に達した場合、ユーザーはそれより多くのアイテムをアーカイブメールボックスに移動することはできません。 サイズ制限に達した後、Office 365 はアーカイブメールボックスのサイズを拡大しません。 代わりに、ユーザーは次の操作を実行して、アーカイブメールボックス内の空き領域を増やすことができます。

- Outlook を使用してアイテムを .pst ファイルにエクスポートする

- アーカイブメールボックスからアイテムを削除します。

Office 365 では、Office 365 Enterprise E3 および E5 のライセンスに対して**無制限のアーカイブ**が提供されています。 管理者は、アーカイブメールボックスが最大サイズに達する前に、この機能を有効にする必要があります。 無制限のアーカイブが有効になっている場合は、アーカイブメールボックスに空き領域が追加されるまでに最大で30日かかることがあります。 そのため、管理者はアーカイブメールボックスの空き領域を確認することをお勧めします。これにより、ユーザーは、拡張中にアーカイブメールボックスを引き続き使用できます。 詳細については、「office [365 での無制限アーカイブの概要](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving)」および「 [office 365 で無制限アーカイブを有効にする](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)」を参照してください。

Outlook からアーカイブメールボックスにアクセスする方法の詳細については、「[自動拡張アーカイブのアイテムにアクセスするための outlook 要件](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)」を参照してください。 アイテムをアーカイブメールボックスに自動的に移動するアイテム保持ポリシーを構成するには、「 [Office 365 組織のメールボックスのアーカイブおよび削除ポリシーをセットアップ](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)する」を参照してください。

**注**: 自動拡張アーカイブは、Exchange 2010 のプライマリメールボックスではサポートされていません。
