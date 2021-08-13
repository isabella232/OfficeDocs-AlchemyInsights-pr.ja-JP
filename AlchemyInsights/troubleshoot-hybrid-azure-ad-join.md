---
title: ハイブリッド Azure AD 参加のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939276"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>ハイブリッド Azure AD 参加のトラブルシューティング

強く推奨するデバイスが[デバイス登録接続のテスト スクリプト](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)を使用して、システム アカウントでデバイス登録エンド ポイントにアクセスできることを確認します。

1. 初めてデバイス登録を設定する場合は、[Azure Active Directory でのデバイス管理の概要](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)を確認して、Azure AD の制御下でデバイスを取得する方法を確認してください。
1. デバイスを Azure AD に直接登録し、それらを Intune に登録する場合は、[Intune を構成](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)し、最初に[ライセンス](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)を設定していることを確認してください。
1. Azure AD およびオンプレミス AD で操作を実行する権限があることを確認してください。 デバイス登録の設定を管理できるのは、Azure AD のグローバル管理者のみです。 さらに、オンプレミスの Active Directory で自動登録を設定する場合は、Active Directory と AD FS (該当する場合) の管理者である必要があります。

ハイブリッド参加に関する潜在的な問題の解決の詳細については、「ハイブリッド Azure AD 参加をセットアップするための[ハイブリッド参加のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)」を参照してください。Azure AD ポータルを使用したデバイスの管理については、「[ハイブリッド Azure AD に参加した (オンプレミスのドメインに参加した) デバイスのセットアップ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support)」および「[Azure ポータルを使用したデバイスの管理](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

ハイブリッド Azure Active Directory (AD) 参加に関する一般的な問題を解決するには、「[ハイブリッド Azure AD 参加に関するよくある質問](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)」をご覧ください。
