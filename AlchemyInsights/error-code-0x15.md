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
description: リモート デスクトップ サービス (RDS) 展開上で Office 2013 のライセンス認証中にエラーを受信した場合は、レジストリを編集して ADAL を有効にすることを検討します。
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499387"
---
<span data-ttu-id="025d0-103">リモート デスクトップ サービス (RDS) 展開上で Office 2013 のライセンス認証中にエラーを受信した場合は、レジストリを編集して ADAL を有効にすることを検討します。</span><span class="sxs-lookup"><span data-stu-id="025d0-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="025d0-104">**レジストリ キー**</span><span class="sxs-lookup"><span data-stu-id="025d0-104">**Registry key**</span></span>|<span data-ttu-id="025d0-105">**型**</span><span class="sxs-lookup"><span data-stu-id="025d0-105">**Type**</span></span>|<span data-ttu-id="025d0-106">**値**</span><span class="sxs-lookup"><span data-stu-id="025d0-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="025d0-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="025d0-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="025d0-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="025d0-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="025d0-109">1</span><span class="sxs-lookup"><span data-stu-id="025d0-109">1</span></span>  <br/> |
   
<span data-ttu-id="025d0-110">詳細については、「[Windows デバイスの Office 2013 の先進認証を有効にする](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="025d0-110">Enable Modern Authentication for Office 2013 on Windows devices</span></span>
  
> [!NOTE]
>  <span data-ttu-id="025d0-p101">ADAL は既定では、Office 365 ProPlus と Office 2016 によって有効になります。> リモート デスクトップ サービス (RDS) は以前、ターミナル サービスと呼ばれていました。</span><span class="sxs-lookup"><span data-stu-id="025d0-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

