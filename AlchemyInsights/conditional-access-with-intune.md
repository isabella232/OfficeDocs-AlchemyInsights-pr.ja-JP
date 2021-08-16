---
title: Intune での条件付きアクセス
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069717"
---
# <a name="conditional-access-with-intune"></a>Intune での条件付きアクセス

Intune で **条件付きアクセス** を使用するには、次の 3 つの手順が必要です。

- **コンプライアンス ポリシー** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android)、[iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)、[Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) を作成して、デバイスが準拠していると見なされるよう満たす必要がある設定を定義します。たとえば、準拠と見なされるには、デバイスには少なくとも 6 桁の暗証番号が必要です。
- 保護されているリソース、およびそれらのリソースにアクセスするために満たす必要がある条件を定義する、**条件付きアクセス ポリシー** を作成します。[たとえば、](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)企業メールにアクセスする前に、デバイスを準拠させる必要があります。
- **コンプライアンス ポリシー** と **条件付きアクセス ポリシー** の両方を確認することは、目的のユーザーのグループを対象としています。これには、Azure Active Directory のユーザーで特定のグループを作成することが必要な場合があります。

**便利なリンク:**

[デバイス コンプライアンスの概要](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA のトラブルシューティング](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[トラブルシューティング ポリシー](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

準拠していないデバイスによるアクセスからメール (Exchange online) を保護するには、両方のドキュメントに従う必要があります。

1. [EAS を使用してデバイスからメール アクセスを保護する](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Outlook などの先進認証クライアントを使用して、デバイスからメール アクセスを保護する](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)