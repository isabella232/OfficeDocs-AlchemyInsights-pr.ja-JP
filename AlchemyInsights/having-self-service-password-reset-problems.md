---
title: セルフサービス パスワード リセット (SSPR) に問題がある場合
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002464"
- "7663"
ms.openlocfilehash: 4f1f94be299c980a6a359d727fb24f411f98b785
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722210"
---
# <a name="having-self-service-password-reset-sspr-problems"></a>セルフサービス パスワード リセット (SSPR) に問題がある場合

ハイブリッド クラウドとオンプレミス環境におけるセルフサービス パスワード リセット (SSPR) の一般的な問題は次のとおりです。

- [SSPR のパスワード ライトバックが有効になっていない](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)
- [Azure AD Premium ライセンスが割り当てられていない](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing)
- [Azure AD Connect の問題](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) or [networking issues](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-connectivity)
- [SSPR の認証方式が登録されていない](https://mysignins.microsoft.com/security-info)
- Microsoft 365 管理センターまたは SSPR を使用している管理者などの、[サポートされていないライトバック シナリオ](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-writeback#unsupported-writeback-operations) 


詳しくは、以下を参照してください。

- [セルフサービス パスワード リセットのトラブルシューティング](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr)
- [Azure Active Directory でのセルフサービス パスワード リセットのトラブルシューティング](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)
