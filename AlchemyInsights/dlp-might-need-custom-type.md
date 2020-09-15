---
title: DLP のカスタム タイプの必要性
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712189"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP のカスタム タイプの必要性

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

**DLP にはカスタム情報の種類が必要な場合があります**

データ損失防止（DLP）ポリシーを使用すると、組織内の機密データを識別し保護することができます。 場合によっては、組織のデータを保護するために独自の**カスタム**機密情報の種類を作成する必要があります。

たとえば、組織では、固有の形式で従業員 ID やその他のデータを識別して保護する必要があることがあります。もしそうであれば、詳細について以下の記事を参照してください。
  
 **組み込みの機密情報の種類をカスタマイズする**
  
組み込みの機密情報の種類がほんの数回の調整でニーズを満たすとすれば、[組み込みの機密情報の種類はカスタマイズできます](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)。 たとえば、キーワードを追加または削除したり、日付や住所などの裏付けとなる証拠を追加または削除したりできます。
  
 **カスタムの機密情報の種類を作成する**
  
ですが、異なる種類の機密情報をすべて識別して保護する必要がある場合は、セキュリティ ＆ コンプライアンス センターの UI で[カスタムの機密情報の種類](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)を作成できます。
  
**セキュリティ ＆ コンプライアンス センター PowerShell でカスタムの機密情報の種類を作成する**

最後に、UI が必要なオプションをすべて提供していない場合は、[ セキュリティ ＆ コンプライアンス センター PowerShell でカスタムの機密情報の種類を作成](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)できます。 XML ファイルを使って始めると、利用可能なすべてのオプションを使用できます。
