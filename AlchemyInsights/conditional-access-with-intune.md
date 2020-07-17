---
title: Intune での条件付きアクセス
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931441"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="01f51-102">Intune での条件付きアクセス</span><span class="sxs-lookup"><span data-stu-id="01f51-102">Conditional Access with Intune</span></span>

<span data-ttu-id="01f51-103">Intune で **条件付きアクセス** を使用するには、次の 3 つの手順が必要です。</span><span class="sxs-lookup"><span data-stu-id="01f51-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="01f51-104">**コンプライアンス ポリシー** を作成し ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows))、デバイスが準拠しているとみなされるために満たす必要がある設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="01f51-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="01f51-105">たとえば、準拠していると見なされるには、デバイスには少なくとも 6 桁の暗証番号 (pin) が必要です。</span><span class="sxs-lookup"><span data-stu-id="01f51-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="01f51-106">**条件付きアクセス ポリシー**を作成し、どのリソースを保護し、リソースへのアクセスにはどのような条件が必要かを定義します。</span><span class="sxs-lookup"><span data-stu-id="01f51-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="01f51-107">[たとえば、](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) 企業のメールにアクセスするにはデバイスが準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="01f51-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="01f51-p103">**コンプライアンス ポリシー** と **条件付きアクセス ポリシー** の両方を確認することは、目的のユーザーのグループを対象としています。これには、Azure Active Directory のユーザーで特定のグループを作成することが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="01f51-p103">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="01f51-110">**便利なリンク:**</span><span class="sxs-lookup"><span data-stu-id="01f51-110">**Helpful links:**</span></span>

[<span data-ttu-id="01f51-111">デバイス コンプライアンスの概要</span><span class="sxs-lookup"><span data-stu-id="01f51-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="01f51-112">CA のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="01f51-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="01f51-113">トラブルシューティング ポリシー</span><span class="sxs-lookup"><span data-stu-id="01f51-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="01f51-114">準拠していないデバイスによるアクセスからメール (Exchange online) を保護するには、両方のドキュメントに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="01f51-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="01f51-115">EAS を使用してデバイスからメール アクセスを保護する</span><span class="sxs-lookup"><span data-stu-id="01f51-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="01f51-116">Outlook などの先進認証クライアントを使用して、デバイスからメール アクセスを保護する</span><span class="sxs-lookup"><span data-stu-id="01f51-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)