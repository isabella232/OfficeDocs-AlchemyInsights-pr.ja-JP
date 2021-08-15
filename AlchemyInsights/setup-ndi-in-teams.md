---
title: NDI テクノロジを有効にする
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023527"
---
# <a name="turn-on-ndi-technology"></a>NDI テクノロジを有効にする

NDI テクノロジでは、ユーザーに対して次の 2 つの手順を有効にする必要があります。

1. テナント管理者が CsTeamsMeetingPolicy で「AllowNDIStreaming」プロパティを有効にする必要があります。

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. この変更が設定された後、エンド ユーザーは、**[設定]、[アクセス許可]** の順に移動して特定のクライアントの NDI® テクノロジを有効にする必要があります。

詳細については、「[Microsoft Teams で NDI テクノロジを使用する](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)」を参照してください。
