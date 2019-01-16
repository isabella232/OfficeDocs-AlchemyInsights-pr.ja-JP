---
title: 設置、フェデレーション サービスの証明書のいずれかが期限切れにします。
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297283"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>設置、フェデレーション サービスの証明書のいずれかが期限切れにします。

この問題を解決するには、次の手順を実行します。
  
- (モジュールがまだインストールされていない) 場合は、コンピューターに、Microsoft Azure Active Directory モジュールの Windows PowerShell をインストールします。[グラフのアクティブなディレクトリの PowerShell を Azure](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)にはこれを行うには、
    
- 手順に従います、「シナリオ 1: AD FS トークン署名証明書の有効期限が切れて」[から AD FS のフェデレーション ユーザーが Office 365 Azure Intune にサインインするときの「サイトへアクセス問題が発生しました」エラー](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)のセクション。
    
- T[を更新または、Office 365、Azure、Intune のフェデレーション ドメインの設定を修復する方法](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)の手順を実行します。
    
フェデレーション証明書の更新の詳細については、 [O365 と Azure AD の証明書の更新](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs)を参照してください。
  

