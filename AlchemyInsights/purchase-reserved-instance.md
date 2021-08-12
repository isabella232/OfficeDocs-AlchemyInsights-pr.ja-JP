---
title: 予約インスタンスの購入
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6816"
ms.openlocfilehash: fc8972d56ad63ac1d0bc16910ed74c7121aefb05f786fdd60a77ba89867d1741
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973054"
---
# <a name="questions-before-purchase"></a>購入前の質問

**既存のリソースに対して予約割引を適用するには、どうすればいいですか?**  
予約特典は、予約 SKU、地域、および範囲と一致する既存のリソースに自動的に適用されます。 リソースに対する予約のタグ付けはありません。 [詳細情報](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support#how-reservation-discount-is-applied) 

**どの仮想マシンを購入すればいいですか?**  
こちらの「[購入前に適正な仮想マシンのサイズを判断する](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?toc=/azure/billing/TOC.json&WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)」の記事を読んでください。

**SQL の予約容量を購入する方法について、質問があります。**  
こちらの「[SQL データベースの予約容量を購入する](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity?toc=/azure/billing/TOC.json&WT.mc_id=Portal-Microsoft_Azure_Support#buy-sql-database-reserved-capacity)」の記事を読んでください。

**間接的な EA カスタマーなのですが、パートナーがいないと購入できませんか?**  
いいえ。 EA サブスクリプションの所有者であれば、RI を購入できます。

**RI の購入は金額コミットメントから控除されますか?**  
はい。金額コミットメントが十分でない場合は、使用可能な金額コミットメントを超過する金額の料金の請求が行われます。

**予約インスタンスは Windows VM か SQL IP コストのどちらに適用されますか?**  
予約インスタンスの割引は、コンピューティングの使用状況にのみ適用されます。 Windows IP コストまたは SQL IP コストは個別に課金され、RI 割引は取得できません。 [Azure Reserved VM Instances を含まないソフトウェア コスト](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs?WT.mc_id=Portal-Microsoft_Azure_Support)  
      
**予約インスタンスの購入に対する課金**  
      
予約インスタンス購入は、購入時点で選択したサブスクリプションに紐付いた支払方法で課金されます。 サブスクリプションの種類は、エンタープライズ契約 (オファー番号: MS-AZR-0017P)、従量課金制 (オファー番号: MS-AZR-0003P)、Microsoft 顧客契約、または CSP にする必要があります。

-   エンタープライズ サブスクリプションでは、料金が登録した金額コミットメント残高から控除されるか、または過剰として請求されます
-   従量課金制サブスクリプションを利用する場合は、サブスクリプションのクレジットカードまたは請求書による支払い方法で料金が請求されます

**サービス プランの購入は、次のとおりです。**

-   [Cosmos DB 予約容量に対する前払い](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity?WT.mc_id=Portal-Microsoft_Azure_Support)
-   [Azure SQL Database 予約容量を使用して SQL データベース コンピューティング リソースへの前払いを行う](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity?WT.mc_id=Portal-Microsoft_Azure_Support)
-   [Azure Reserved VM Instances を使用して仮想マシンへの前払いを行う](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support)

**ソフトウェア プランの購入は、次のとおりです。**

-   [Azure 予約から Red Hat ソフトウェア プランへの前払いを行う](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-rhel-software-charges?WT.mc_id=Portal-Microsoft_Azure_Support)
-   [Azure 予約から SUSE ソフトウェア プランへの前払いを行う](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges?WT.mc_id=Portal-Microsoft_Azure_Support)