---
title: Teams のウェビナーを有効にする
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794246"
---
# <a name="enable-teams-webinars"></a>Teams のウェビナーを有効にする

ウェビナーは既定で有効になっています。 Teams Powershell コマンドを使用して、スケジュールを行ってTeams ウェビナーに登録できるユーザーを管理します。

- 会議を作成できるすべてのユーザーは、ウェビナー会議を作成することもできます。 Teams ウェビナーをスケジュールできるユーザーを管理する場合は、*AllowMeetingRegistration* を使用します。 
- 既定では、*WhoCanRegister* が有効になっており、[**Everyone**] に設定されています。 会議の登録を無効にする場合は、*AllowMeetingRegistration* を **False** に設定します。

これらの設定を変更するには、[Teams PowerShell](/microsoftteams/teams-powershell-install) をインストールする必要があります。 また、会議ポリシーが Teams ウェビナーに適用されます。 たとえば、会議の設定で匿名参加がオフになっている場合、匿名ユーザーはウェビナーに参加できません。

ウェビナーに登録できるユーザーの構成の詳細については、「[ウェビナーに登録できるユーザーを構成する](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)」 を参照してください。 Microsoft Lists の設定の詳細については、「 [Microsoft Lists のコントロール設定」](/sharepoint/control-lists)を参照してください。