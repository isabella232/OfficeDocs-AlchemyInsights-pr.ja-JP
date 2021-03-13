---
title: Intune での条件付きアクセスの使用
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751314"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="31cec-102">Intune での条件付きアクセスの使用</span><span class="sxs-lookup"><span data-stu-id="31cec-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="31cec-103">Intune で条件付きアクセスを使用するには、次の 3 つの手順が必要です。</span><span class="sxs-lookup"><span data-stu-id="31cec-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="31cec-104">コンプライアンス ポリシーを作成して、デバイスが準拠していると見なされるよう満たす必要がある設定を定義します。たとえば、準拠と見なされるには、デバイスには少なくとも 6 桁の暗証番号が必要です。</span><span class="sxs-lookup"><span data-stu-id="31cec-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="31cec-105">保護されているリソース、およびそれらのリソースにアクセスするために満たす必要がある条件を定義する、条件付きアクセス ポリシーを作成します。たとえば、企業メールにアクセスする前に、デバイスを準拠させる必要があります。</span><span class="sxs-lookup"><span data-stu-id="31cec-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="31cec-106">コンプライアンス ポリシーと条件付きアクセス ポリシーの両方で、目的のグループのユーザーが対象となるように設定します。これを行うには、Azure Active Directory で特定のユーザー グループを作成する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="31cec-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="31cec-107">続きを読む</span><span class="sxs-lookup"><span data-stu-id="31cec-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
