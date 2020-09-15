---
title: SharePoint、OneDrive、Microsoft Teams 用の ATP
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715566"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>SharePoint、OneDrive、Microsoft Teams 用の ATP

次の手順を実行して、Advanced Threat Protection を有効にします。

1. [https://protection.office.com](https://protection.office.com) に移動して、全体管理者またはセキュリティ管理者のアカウントでサインインします。

2. 左側のナビゲーション ウィンドウにある **[脅威の管理]** で、**[ポリシー]** \> **[安全な添付ファイル]** を選択します。

3. **[SharePoint、OneDrive、および Microsoft Teams に対して ATP を有効にする]** をオンにします。

4. [アクティビティ アラート ポリシーを作成](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts)して、悪意のあるファイルが検出されたときに通知を受け取るようにします。

詳細な手順については、この[トピック](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)を参照してください。

**注**: ATP は、SharePoint Online、OneDrive for Business、または Microsoft Teams のファイルを 1 つずつスキャンしないようになっています。 ファイルは、共有のアクティビティ、ゲストのアクティビティ、および脅威のシグナルを使用して悪意のあるファイルを特定するプロセスによって、非同期的にスキャンされます。 詳細については、この[トピック](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)を参照してください。
