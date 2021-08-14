---
title: SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 9051fb44d7d6bde388d279b3311627848b6f499e30b5eca00d6a47cef105fb77
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997139"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365

次の手順に従って、Microsoft Defender for Office 365 を有効にします。

1. [https://protection.office.com](https://protection.office.com) に移動して、全体管理者またはセキュリティ管理者のアカウントでサインインします。

2. 左側のナビゲーション ウィンドウにある **[脅威の管理]** で、**[ポリシー]** \> **[安全な添付ファイル]** を選択します。

3. **[SharePoint、OneDrive、Microsoft Teams 用の Defender for Office 365 を有効にする]** を選択します。

4. [アクティビティ アラート ポリシーを作成](/microsoft-365/compliance/create-activity-alerts)して、悪意のあるファイルが検出されたときに通知を受け取るようにします。

詳細な手順については、「[SharePoint、OneDrive、Microsoft Teams に対して安全な添付ファイルをオンにする](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)」を参照してください。

**注**: Microsoft Defender for Office 365 は、SharePoint Online、OneDrive for Business、または Microsoft Teams のファイルを 1 つずつスキャンしないようになっています。 ファイルは、共有のアクティビティ、ゲストのアクティビティ、および脅威のシグナルを使用して悪意のあるファイルを特定するプロセスによって、非同期的にスキャンされます。 詳細については、「[SharePoint、OneDrive、Microsoft Teams の安全な添付ファイル](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)」を参照してください。
