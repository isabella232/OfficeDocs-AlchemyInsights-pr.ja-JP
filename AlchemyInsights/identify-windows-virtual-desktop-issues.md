---
title: Windows Virtual Desktop の問題を特定する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 398496448089d4480119a2eb21221dc11f13c6c1f3bcbd931d6c18033f2e734e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53987554"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Windows Virtual Desktop の問題を特定する

Windows Virtual Desktop の診断では、1 つの Powershell コマンドレットを使用しますが、オプションのパラメータがたくさんあり、これにより問題を絞り込んで特定します。 

1. Windows Virtual Desktop PowerShell モジュールをダウンロードしてインポートします。 詳細については、「[Windows PowerShell の Windows Virtual Desktop コマンドレット](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)」を参照してください。

1. 次のコマンドレットを実行して、アカウントにサインインします。
    
    例: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**注意:** PowerShell を使用するすべてのクエリは、-UserName または -ActivityID パラメーターのいずれかを含める必要があります。 監視機能の詳細については、「[診断機能の Log Analytics](https://go.microsoft.com/fwlink/?linkid=2126847) を使用する」を参照してください。

ユーザー別に診断アクティビティをフィルター処理するには、次のコマンドレットを実行します。

例: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

問題を診断するのに実行するフィルターの一覧です。 問題の診断の詳細については、「[Windows Virtual Desktop の問題を特定して診断する](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) を参照してください。

一般的なエラーの詳細については、「[一般的なエラーのシナリオ](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)」を参照してください。
