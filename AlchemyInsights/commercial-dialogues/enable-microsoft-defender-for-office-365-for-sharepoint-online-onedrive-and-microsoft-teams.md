---
title: オンライン、セーフ、SharePointの添付ファイルOneDrive有効Microsoft Teams
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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332384"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>オンライン、セーフ、SharePointの添付ファイルOneDrive有効Microsoft Teams

1. グローバル管理者またはセキュリティ管理者の資格情報を使用して、Microsoft 365 Defender ポータルを開き、[ポリシー] セクションの [ポリシー & ルールの脅威ポリシーセーフ添付ファイル] に <https://security.microsoft.com>  \>  \> **移動** します。

   [添付ファイル] ページに **直接移動セーフを** 使用します <https://security.microsoft.com/safeattachmentv2> 。

2. [添付ファイル **セーフ] ページで**、[グローバル設定]**をクリックします**。
3. 表示されるフライアウトで **、[SharePoint、OneDrive、** および Microsoft Teams に対して Microsoft Office 365 Defender を有効にする] を選択し、[保存] を選択 **します**。

    **ヒント**: 次の手順を実行して、添付ファイルの保護を強化セーフ、SharePoint、OneDrive、Microsoft Teams。
    - ユーザーが悪意のあるファイルをダウンロードするのを防ぐには `$true` 、SharePoint Online PowerShell の **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** コマンドレットの *DisallowInfectedFileDownload* パラメーターの値を使用します。 詳細については、「Use SharePoint Online PowerShell を使用して、ユーザーが悪意のある[ファイルをダウンロードするを防ぐ」を参照してください](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)。
    - [検出されたファイルのアラート ポリシーを作成する](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

詳細については、「添付ファイル[セーフOffice 365、SharePoint、OneDrive」を参照Microsoft Teams。](https://go.microsoft.com/fwlink/?linkid=2092041)
