---
title: Intune で条件付きのアクセス
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297212"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="04904-102">Intune で条件付きのアクセス</span><span class="sxs-lookup"><span data-stu-id="04904-102">Conditional Access with Intune</span></span>

<span data-ttu-id="04904-103">Intune で**条件付きのアクセス**を使用するには、3 つの手順が必要です。</span><span class="sxs-lookup"><span data-stu-id="04904-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="04904-p101">どのようなリソースが保護されていると、条件は満たす必要があるこれらのリソースにアクセスする必要がある**条件付きのアクセス ポリシー**を作成します。などのデバイスは、企業の電子メールにアクセスする前に準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="04904-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="04904-p102">デバイスは準拠と見なされる前に満たす必要のある設定を定義するための**コンプライアンス ・ ポリシー**を作成します。などのデバイスは、準拠と見なされる前に、少なくとも 6 桁の暗証番号 (pin) が必要です。</span><span class="sxs-lookup"><span data-stu-id="04904-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="04904-p103">**コンプライアンス ・ ポリシー**と**アクセス ポリシーの条件**の両方が必要なユーザーのグループを対象としたことを確認します。Azure Active Directory 内の特定のユーザー グループを作成するこの必要があります。</span><span class="sxs-lookup"><span data-stu-id="04904-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="04904-110">詳細を表示します。</span><span class="sxs-lookup"><span data-stu-id="04904-110">Read more:</span></span>
  
- [<span data-ttu-id="04904-111">条件付きアクセスのベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="04904-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="04904-112">条件付きアクセスの概要</span><span class="sxs-lookup"><span data-stu-id="04904-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

