---
title: エラー コード 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: リモート デスクトップ サービス (RDS) 展開上で Office 2013 のライセンス認証中にエラーを受信した場合は、レジストリを編集して ADAL を有効にすることを検討します。
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929093"
---
<span data-ttu-id="abe38-103">リモート デスクトップ サービス (RDS) 展開上で Office 2013 のライセンス認証中にエラーを受信した場合は、レジストリを編集して ADAL を有効にすることを検討します。</span><span class="sxs-lookup"><span data-stu-id="abe38-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="abe38-104">**レジストリ キー**</span><span class="sxs-lookup"><span data-stu-id="abe38-104">**Registry key**</span></span>|<span data-ttu-id="abe38-105">**型**</span><span class="sxs-lookup"><span data-stu-id="abe38-105">**Type**</span></span>|<span data-ttu-id="abe38-106">**値**</span><span class="sxs-lookup"><span data-stu-id="abe38-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="abe38-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="abe38-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="abe38-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="abe38-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="abe38-109">1</span><span class="sxs-lookup"><span data-stu-id="abe38-109">1</span></span>  <br/> |
   
<span data-ttu-id="abe38-110">詳細については、「[Windows デバイスの Office 2013 の先進認証を有効にする](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abe38-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="abe38-p101">ADAL は既定では、Office 365 ProPlus と Office 2016 によって有効になります。> リモート デスクトップ サービス (RDS) は以前、ターミナル サービスと呼ばれていました。</span><span class="sxs-lookup"><span data-stu-id="abe38-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

