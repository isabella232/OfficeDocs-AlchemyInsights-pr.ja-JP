---
title: SharePoint、OneDrive、Microsoft Teams の Office 365 ATP を有効にする
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801054"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint、OneDrive、Microsoft Teams の Microsoft Defender for Office 365 を有効にする

1. https://protection.office.com に移動し、サインインします。
2. **脅威管理** > **ポリシー** > **安全な添付ファイル** を選択します。
3. [ **ATP を SharePoint、OneDrive、Microsoft Teams で有効にする** ]を選択し、[ **保存** ]をクリックします。
4. (推奨) グローバル管理者または SharePoint Online 管理者として、 **DisallowInfectedFileDownload** パラメーターを *true* に設定して [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) コマンドレットを実行します。
5. (推奨) 検出されたファイルに対する[警告を設定](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)します。

> [!NOTE]
> ATP は SharePoint Online、OneDrive、または Microsoft Teams のすべてのファイルをスキャンしません。 ファイルは、共有イベントおよびゲスト アクティビティ イベントをスマート ヒューリスティックおよび脅威のシグナルと共に使用して悪質なファイルを特定するプロセスを通じて、非同期的にスキャンされます。 「[SharePoint、OneDrive、Microsoft Teams 用の ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)」を参照してください。