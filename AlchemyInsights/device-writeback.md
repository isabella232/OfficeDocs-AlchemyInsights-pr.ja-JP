---
title: デバイスの書き戻し
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320091"
---
# <a name="device-writeback"></a>デバイスの書き戻し

デバイスの書き戻しは、次のようなシナリオで使用します。

- [ハイブリッド証明書信頼の展開を使用した Windows Hello for Business ](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)を有効にします。
- ADFS (2012 R2 以降) で保護されたアプリケーション (証明書利用者の信頼) へのデバイスに基づく条件付きアクセスを有効にします。

    **注**: デバイスの書き戻しAzure AD Premiumに必要なサブスクリプションです。

これにより、セキュリティが強化され、アプリケーションへのアクセスが信頼されたデバイスに対してのみ許可されることが保証されます。 条件付きアクセスの詳細については、「[条件付きアクセス ポリシーを使用したリスクの管理](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)」と「[Azure Active Directory Device Registration を使用したオンプレミスの条件付きアクセスの設定](https://docs.microsoft.com/azure/active-directory/devices/overview)」を参照してください。

デバイスの書き戻しの有効化に関する詳細については、「[デバイスの書き戻しを有効にする](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)」を参照してください。
