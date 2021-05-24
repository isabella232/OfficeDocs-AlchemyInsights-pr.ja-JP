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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543933"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint、OneDrive、Microsoft Teams の Microsoft Defender for Office 365 を有効にする

1. https://protection.office.com に移動し、サインインします。
2. **脅威管理** > **ポリシー** > **安全な添付ファイル** を選択します。
3. **[SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365 を有効にする]** を選択してから、**[保存]** をクリックします。
4. (推奨) グローバル管理者または SharePoint Online 管理者として、**DisallowInfectedFileDownload** パラメーターを *true* に設定して [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) コマンドレットを実行します。
5. (推奨) 検出されたファイルに対する[警告を設定](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)します。

> [!NOTE]
> Microsoft Defender for Office 365 は、SharePoint Online、OneDrive、Microsoft Teams にあるすべてのファイルをスキャンするわけではありません。 ファイルは、共有イベントおよびゲスト アクティビティ イベントをスマート ヒューリスティックおよび脅威のシグナルと共に使用して悪質なファイルを特定するプロセスを通じて、非同期的にスキャンされます。 「[SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)」を参照してください。