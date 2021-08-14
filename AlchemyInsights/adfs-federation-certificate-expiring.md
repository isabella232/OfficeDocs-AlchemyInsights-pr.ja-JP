---
title: ADFS フェデレーション証明書の期限切れ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952974"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS フェデレーション証明書の期限切れ

この問題を解決するには、次の手順を行います。
  
1. コンピューター上で Windows PowerShell 用 Microsoft Azure Active Directory モジュールをインストールします (モジュールがまだインストールされていない場合)。これを行うには、[Windows PowerShell を使用した Azure AD の管理](https://aka.ms/aadposh)に関するページに移動します。

2. [フェデレーション ユーザーが Microsoft 365、Azure、または Intune にサインインするときに、AD FS から示された「サイトへのアクセスに関する問題が発生しました」エラー](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)の「シナリオ 1: AD FS トークン署名の証明書が失効している」セクションの手順に従います。

3. 「[Microsoft、Azure、または Intune のフェデレーション ドメインの設定を更新または修復する](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)」の手順に従います。

    フェデレーション証明書の更新に関する詳細については、「[Microsoft 365 および Azure Active Directory 用のフェデレーション証明書の更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)」を参照してください。
