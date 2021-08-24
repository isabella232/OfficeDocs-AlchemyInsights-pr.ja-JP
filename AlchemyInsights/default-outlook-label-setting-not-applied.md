---
title: 既定の Outlook ラベル設定が適用されていません
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455394"
---
# <a name="default-outlook-label-setting-not-applied"></a>既定の Outlook ラベル設定が適用されていません

Outlook の既定のラベル設定が正しく適用されておらず、別のラベルが適用されているか、またはラベルが適用されていない場合は、既知の問題 (MC277818) が発生している可能性があります。問題を解決するには、次の 2 つのオプションのいずれかを実行する必要があります。

**オプション 1:**

1. Microsoft 365 コンプライアンス センター > **Solutions** > **Information Protection** に移動します。
1. **［ラベル ポリシー］** を選択して、編集する必要があるラベル ポリシーを選択します (**OutlookDefaultlabel** 設定が問題のラベル ポリシーに正しく設定されていません。 **Get-labelpolicy** を実行して、この設定を表示し)、**［ポリシーの編集**］ を選択します。
1. [**このデフォルトのラベルを電子メールに適用する**] 設定が表示されるまで、[**次へ**] を選択します。この設定は、 [**ポリシー設定**] ダイアログ ボックスで、[**ユーザーにメールとドキュメントへのラベルの適用を要求する**] を選択した場合に使用できます。
1. [**ドキュメントにデフォルトのラベルを適用する**] ダイアログボックスで、ドロップダウン リストから [**なし**] を選択します。 
1. [**次へ**] と [**送信**] を選択して、ラベル設定を保存します。 

**オプション 2:**

[セキュリティとコンプライアンス センター Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps) で、Set-LabelPolicy コマンドレットを使用して、{OutlookDefaultLabel = "None"} で **OutlookDefaultlabel** を **［なし］** に変更します。

次を実行します: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Outlook の既定のラベルの詳細については、「[Outlook に別の既定のラベルを設定する](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)」をご覧ください。