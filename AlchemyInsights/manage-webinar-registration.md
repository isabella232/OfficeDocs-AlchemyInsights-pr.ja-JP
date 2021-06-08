---
title: ウェビナー登録の管理
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798649"
---
# <a name="manage-webinar-registration"></a>ウェビナー登録の管理

Teams Powershell コマンドを使用して、Teams ウェビナーに登録できるユーザーを管理します。 Teams PowerShell をインストールするには、「[Teams PowerShell](/microsoftteams/teams-powershell-install)」を参照してください。 

既定では、*WhoCanRegister* が有効になっており、[**Everyone**] に設定されています。 

会議出席依頼にすべてのユーザー の登録を許可するオプションが表示されない場合は、*WhoCanRegister* 設定を [すべてのユーザー] に再実行し、24 時間待ちます。 *WhoCanRegister* を再実行するには、Powershell コマンドを使用します。

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**注**: 会議の設定で匿名参加がオフになっている場合、匿名ユーザーはウェビナーに参加できません。 この設定の詳細と有効化については、「[Microsoft Teams で会議設定を管理する](/microsoftteams/meeting-settings-in-teams)」を参照してください。

会議の登録を無効にする場合は、*AllowMeetingRegistration* を **False** に設定します。

ウェビナーに登録できるユーザーの構成の詳細については、「[ウェビナーに登録できるユーザーを構成する](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)」 を参照してください。 Microsoft Lists の設定の詳細については、「 [Microsoft Lists のコントロール設定」](/sharepoint/control-lists)を参照してください。
