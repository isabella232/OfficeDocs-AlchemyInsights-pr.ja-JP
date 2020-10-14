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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709912"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint、OneDrive、Microsoft Teams の Office 365 Advanced Threat Protection を有効にする

1. https://protection.office.com に移動し、サインインします。
2. **脅威管理** > **ポリシー** > **安全な添付ファイル**を選択します。
3. [**ATP を SharePoint、OneDrive、Microsoft Teams で有効にする**]を選択し、[**保存**]をクリックします。
4. (推奨) グローバル管理者または SharePoint Online 管理者として、**DisallowInfectedFileDownload** パラメーターを *true* に設定して [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) コマンドレットを実行します。
5. (推奨) 検出されたファイルに対する[警告を設定](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)します。

> [!NOTE]
> ATP は SharePoint Online、OneDrive、または Microsoft Teams のすべてのファイルをスキャンしません。 ファイルは、共有イベントおよびゲスト アクティビティ イベントをスマート ヒューリスティックおよび脅威のシグナルと共に使用して悪質なファイルを特定するプロセスを通じて、非同期的にスキャンされます。 「[SharePoint、OneDrive、Microsoft Teams 用の ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)」を参照してください。