---
title: エラー コード 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: リモート デスクトップ サービス (RDS) の展開で Office 2013 をアクティブ化中にエラーを発生する場合は、レジストリを編集して ADAL を有効にすることを検討してください。
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499387"
---
<span data-ttu-id="194fa-103">リモート デスクトップ サービス (RDS) の展開で Office 2013 をアクティブ化中にエラーを発生する場合は、レジストリを編集して ADAL を有効にすることを検討してください。</span><span class="sxs-lookup"><span data-stu-id="194fa-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="194fa-104">**レジストリ キー**</span><span class="sxs-lookup"><span data-stu-id="194fa-104">**Registry key**</span></span>|<span data-ttu-id="194fa-105">**タイプ**</span><span class="sxs-lookup"><span data-stu-id="194fa-105">**Type**</span></span>|<span data-ttu-id="194fa-106">**値**</span><span class="sxs-lookup"><span data-stu-id="194fa-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="194fa-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="194fa-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="194fa-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="194fa-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="194fa-109">1</span><span class="sxs-lookup"><span data-stu-id="194fa-109">1</span></span>  <br/> |
   
<span data-ttu-id="194fa-110">詳細については、 [Windows デバイスでの Office 2013 の最新認証を有効にする](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="194fa-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="194fa-p101">ADAL は、Office 365 用リソースおよび 2016 の Office で既定で有効になります。以前 _gt リモート デスクトップ サービス (RDS) ターミナル サービスの名前は。</span><span class="sxs-lookup"><span data-stu-id="194fa-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

