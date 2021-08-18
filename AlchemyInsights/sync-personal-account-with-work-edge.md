---
title: ユーザーが個人用アカウントを Microsoft Edge の職場アカウントと同期できるようにする
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: ad4b64c4bb50f50d4ab9fa47bb37228dce538e6d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317283"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>ユーザーが個人用アカウントを Microsoft Edge の職場アカウントと同期できるようにする

次の条件を満たしていることを確認します:

- Enterprise State Roamingは、Azure Active Directory 管理センターで有効になっています。これには、Azure Active Directory Premium または Enterprise Mobility + Security (EMS) のサブスクリプションが必要です。 詳細については、「[Azure Active Directory で Enterprise State Roaming を有効にする](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-enable)」を参照してください。
- 次の条件のいずれかまたは両方を満たしています。
    - Azure Information Protection サービスはテナントに対して有効になっています。 詳細については、「[Azure Rights Management protection を Microsoft 365 管理センターからアクティブ化する](https://docs.microsoft.com/azure/information-protection/activate-office365)」を参照してください。
    - Azure Active Directory Enterprise State Roaming (ESR) 機能は、すべてのユーザーまたはテナントに対して有効になっています。 詳細については、「[エンタープライズ状態ローミングとは](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview)」を参照してください。

AIP と ESR が両方無効になっている場合は、アカウントの同期が利用できないことをユーザーに通知するエラー メッセージが表示されます。
