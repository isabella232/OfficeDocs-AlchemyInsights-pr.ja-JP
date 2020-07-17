---
title: エラー コード 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: リモート デスクトップ サービス (RDS) 展開上で Office 2013 のライセンス認証中にエラーを受信した場合は、レジストリを編集して ADAL を有効にすることを検討します。
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506851"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="539b9-103">リモート デスクトップ サービスで Office 2013 のライセンス認証中に発生するエラー</span><span class="sxs-lookup"><span data-stu-id="539b9-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="539b9-104">リモート デスクトップ サービス (RDS) 展開上で Office 2013 のライセンス認証中にエラーを受信した場合は、レジストリを編集して ADAL を有効にすることを検討します。</span><span class="sxs-lookup"><span data-stu-id="539b9-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="539b9-105">**レジストリ キー**</span><span class="sxs-lookup"><span data-stu-id="539b9-105">**Registry key**</span></span>|<span data-ttu-id="539b9-106">**型**</span><span class="sxs-lookup"><span data-stu-id="539b9-106">**Type**</span></span>|<span data-ttu-id="539b9-107">**値**</span><span class="sxs-lookup"><span data-stu-id="539b9-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="539b9-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="539b9-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="539b9-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="539b9-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="539b9-110">1</span><span class="sxs-lookup"><span data-stu-id="539b9-110">1</span></span>  <br/> |

<span data-ttu-id="539b9-111">詳細については、「[Windows デバイスの Office 2013 の先進認証を有効にする](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="539b9-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="539b9-112">ADAL は、Microsoft 365 Apps for enterprise および Office 2016 で既定で有効になっています。</span><span class="sxs-lookup"><span data-stu-id="539b9-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="539b9-113">リモート デスクトップ サービス (RDS) は以前ターミナル サービスと呼ばれていました。</span><span class="sxs-lookup"><span data-stu-id="539b9-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  