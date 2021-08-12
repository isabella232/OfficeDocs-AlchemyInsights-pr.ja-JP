---
title: ハイブリッド Azure AD 参加のトラブルシューティング
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939924"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>ハイブリッド Azure AD 参加のトラブルシューティング

1. 初めてデバイス登録を設定する場合は、「[Azure Active Directory でのデバイス管理の概要](https://docs.microsoft.com/azure/active-directory/devices/overview)」を確認してください。このガイドでは、デバイスを Azure AD の制御下に配置する方法について説明しています。 
1. デバイスを Azure AD に直接登録し、それらを Intune に登録する場合は、[構成済み Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) があり、最初に[ライセンス](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)が設定されていることを確認する必要があります。
1. Azure AD で操作を実行する権限があることを確認してください。 デバイス登録の設定を管理できるのは、Azure AD のグローバル管理者のみです。
1. Azure AD 参加の実装を行うには、「[Azure AD 参加の計画](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)」を参照してください。

Azure AD 参加に関する一般的な問題の解決の詳細については、「[Azure AD 参加に関するよくある質問](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq)」を参照してください。また、Windows 10 Pro デバイスについては、「[Windows 10 Pro マシンで Azure AD に参加できない - アップグレードする必要がある - Microsoftコミュニティ](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)」を参照してください。
