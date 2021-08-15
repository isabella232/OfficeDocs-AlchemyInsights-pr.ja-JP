---
title: Microsoft Defender Advanced Threat Protection (ATP) から Windows 以外のデバイスをオフボードする
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
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967806"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Microsoft Defender Advanced Threat Protection (ATP) から Windows 以外のデバイスをオフボードする

次の操作を実行してください。

1. サードパーティのソリューションを Microsoft Defender ATP から切断するには、サードパーティのドキュメントに従ってください。
2. Azure Active Directory テナントから、サードパーティのソリューションのアクセス許可を削除します。

    1. [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612) にサインインします。
    1. **[すべてのサービス]** > **[Azure Active Directory]** > **[エンタープライズ アプリケーション]** の順に選択します。
    1. オフボードするアプリケーションを選択します。
    1. **[削除]** を選択します。

詳細については、「[Windows 以外のデバイスをオフボードする](https://go.microsoft.com/fwlink/?linkid=2143630)」を参照してください。
