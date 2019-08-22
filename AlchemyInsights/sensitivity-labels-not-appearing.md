---
title: 機密ラベルが表示されない
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: be5fac4cf4f1516575b8310347dd1d1948010538
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504540"
---
# <a name="sensitivity-labels-not-appearing"></a>機密ラベルが表示されない

機密ラベルを使用すると、機密コンテンツの分類と保護に役立ちます。 この機能の詳細については、「[機密ラベルの概要](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)」を参照してください。

機密ラベルを構成したものの、Office アプリに表示されていない場合は、次の点を確認してください。

- 機密ラベルが必要なユーザーおよびグループに[公開](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do)されていることを確認します。

- ユーザーが機密ラベルをサポートするアプリを使用していることを確認します。[ドキュメントの「機密ラベル](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable)」を参照してください。

- [Azure Information Protection のラベルを移行](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)する場合は、[ここ](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)に記載されている考慮事項に注意してください。

- データ損失防止 (DLP) のサポート: 現在、DLP ポリシーの条件として使用できるのは、保持ラベルのみです。  DLP ポリシーでの機密ラベルのサポートは、まだ利用できませんが、作業中です。

考えられる問題の詳細については、「[既知の問題 (機密ラベル](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc?ui=en-US&rs=en-US&ad=US))」を参照してください。