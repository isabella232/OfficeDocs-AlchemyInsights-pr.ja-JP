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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446696"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP のカスタム タイプの必要性

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

**DLP にはカスタム情報の種類が必要な場合があります**

データ損失防止（DLP）ポリシーを使用すると、組織内の機密データを識別し保護することができます。 場合によっては、組織のデータを保護するために独自のカスタム機密情報の種類を作成する必要があります。 詳細については、「[機密情報の種類に関する詳細](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about)」および「[機密情報の種類のエンティティ定義](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」を参照してください。

カスタムの機密情報の種類とポリシーを作成する方法の詳細については、次を参照してください。 

**組み込みの機密情報の種類をカスタマイズする**

組み込みの機密情報の種類がほんの数回の調整でニーズを満たすとすれば、「[組み込みの機密情報の種類をカスタマイズする](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)」を参照してください。 たとえば、キーワードを追加または削除したり、日付や住所などの裏付けとなる証拠を追加または削除したりできます。

**カスタムの機密情報の種類を作成する**

しかし、異なる種類の機密情報をすべて識別して保護する必要がある場合は、Microsoft 365 コンプライアンス センターでカスタムの機密情報の種類を作成できます。 詳細については、「[カスタムの機密情報の種類の概要](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)」を参照してください。

**セキュリティ/コンプライアンス センター PowerShell でカスタムの機密情報の種類を作成する**

最後に、UI が必要なオプションをすべて提供していない場合は、 セキュリティ/コンプライアンス センター PowerShell でカスタムの機密情報の種類を作成できます。 XML ファイルを使って始めると、利用可能なすべてのオプションを使用できます。 詳細については、「[PowerShell を使用してカスタムの機密情報の種類を作成する](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)」をご覧ください。

最初にテスト モードでポリシーをテストするには「[テスト モードの実装ポリシー](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode)」 および 「[ DLP ポリシーの作成、テスト、調整](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy)」を参照してください。 