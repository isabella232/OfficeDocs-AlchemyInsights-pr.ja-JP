---
title: ADFS フェデレーション証明書の有効期限が切れる
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477216"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS フェデレーション証明書の有効期限が切れる

この問題を解決するには、次の手順を実行します。
  
1. (モジュールがまだインストールされていない) 場合は、コンピューターに、Microsoft Azure Active Directory モジュールの Windows PowerShell をインストールします。これを行うには、 [Windows PowerShell を使用して AD を Azure の管理](https://aka.ms/aadposh)に移動します。
    
2. 手順に従います、「シナリオ 1: AD FS トークン署名証明書の有効期限が切れて」[から AD FS のフェデレーション ユーザーが Office 365 Azure Intune にサインインするときの「サイトへアクセス問題が発生しました」エラー](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)のセクション。
    
3. [更新するか、Office 365、Azure、Intune のフェデレーション ドメインの設定を修復する方法](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)の手順に従います。
    
    フェデレーション証明書の更新に関する詳細については、 [Office 365 と Azure Active Directory フェデレーションの証明書の更新](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs)を参照してください。
    

