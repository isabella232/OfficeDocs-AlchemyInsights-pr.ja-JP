---
title: SharePoint、OneDrive、Microsoft Teams の Microsoft Defender for Office 365 を有効にする
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751197"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint、OneDrive、Microsoft Teams の Microsoft Defender for Office 365 を有効にする

1. グローバル管理者またはセキュリティ管理者の資格情報を使用して、[Office 365 セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインします。
2. 左側のウィンドウで **[脅威の管理]** を選択し、**[ポリシー]** > [[安全な添付ファイル]](https://protection.office.com/safeattachment) の順に選択します。
3. **[SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365 をオンにする]** を選択してから **[保存]** を選択します。
    > [!TIP]
    >
    > - グローバル管理者または SharePoint Online 管理者として、**DisallowInfectedFileDownload** パラメーターを *true* に設定して、次の PowerShell コマンドレットを実行します: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [検出されたファイルに対する警告を設定する](https://go.microsoft.com/fwlink/?linkid=2092110)

詳細については、「[SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092041)」を参照してください。
