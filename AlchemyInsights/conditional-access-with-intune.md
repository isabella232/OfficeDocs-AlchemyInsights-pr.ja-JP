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
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706026"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e74f1-102">Intune での条件付きアクセス</span><span class="sxs-lookup"><span data-stu-id="e74f1-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e74f1-103">Intune で**条件付きアクセス**を使用するには、次の 3 つの手順が必要です。</span><span class="sxs-lookup"><span data-stu-id="e74f1-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="e74f1-p101">保護されているリソース、およびそれらのリソースにアクセスするために満たす必要がある条件を定義する、**条件付きアクセス ポリシー**を作成します。たとえば、企業メールにアクセスする前に、デバイスを準拠させる必要があります。</span><span class="sxs-lookup"><span data-stu-id="e74f1-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="e74f1-p102">**コンプライアンス ポリシー**を作成して、デバイスが準拠していると見なされるよう満たす必要がある設定を定義します。たとえば、準拠と見なされるには、デバイスには少なくとも 6 桁の暗証番号が必要です。</span><span class="sxs-lookup"><span data-stu-id="e74f1-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="e74f1-p103">**コンプライアンス ポリシー**と**条件付きアクセス ポリシー**の両方を確認することは、目的のユーザーのグループを対象としています。これには、Azure Active Directory のユーザーで特定のグループを作成することが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="e74f1-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="e74f1-110">続きを読む:</span><span class="sxs-lookup"><span data-stu-id="e74f1-110">Read more:</span></span>
  
- [<span data-ttu-id="e74f1-111">条件付きアクセスのベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="e74f1-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="e74f1-112">条件付きアクセスの概要</span><span class="sxs-lookup"><span data-stu-id="e74f1-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

