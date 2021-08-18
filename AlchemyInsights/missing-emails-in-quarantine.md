---
title: 検疫されたメールがなくなった場合
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329667"
---
# <a name="missing-emails-in-quarantine"></a>検疫されたメールがなくなった場合

管理者は、[これらのメッセージを表示、解放、または削除](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)できます

<https://security.microsoft.com> の Microsoft 365 Defender ポータルで、**[確認]** \> **[検疫]** の順に移動します。 または、[**検疫**] ページに直接移動するには、<https://security.microsoft.com/quarantine> を使用します。  

使用できる検索/フィルター値の詳細については、「[EOP で管理者として検疫されたメッセージとファイルを管理する](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)」を参照してください。

検疫内のメッセージとファイルを表示および管理するコマンドレットは、次のとおりです。

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): このコマンドレットはメッセージ専用であり、SharePoint、OneDrive、または Microsoft Teams の安全な添付ファイルからのファイルではないことに注意してください。
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
