---
title: 932 AADConnect のアップグレード
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757296"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="75398-102">Azure AD Connect をアップグレードする</span><span class="sxs-lookup"><span data-stu-id="75398-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="75398-p101">既定では、Azure AD Connect の自動アップグレードが有効になっています。これはユーザーが確実に最新バージョンを実行するために役立ちます。自動アップグレードの設定を確認するには、Azure AD PowerShell で **Get-ADSyncAutoUpgrade** コマンドレットを使用します。コマンドレットは次のいずれかの値を返します。</span><span class="sxs-lookup"><span data-stu-id="75398-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="75398-106">**Enabled**: 自動アップグレードが有効になっています。</span><span class="sxs-lookup"><span data-stu-id="75398-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="75398-107">**Disabled**: 自動アップグレードが無効になっています。</span><span class="sxs-lookup"><span data-stu-id="75398-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="75398-p102">**Suspended**: システムが自動アップグレードの受信に対して不適格になっています。この値はシステムによって設定されます。ユーザーが設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="75398-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="75398-110">詳細については、「[自動アップグレード](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75398-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="75398-111">最新バージョンの Azure AD Connect をダウンロードするには、[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) に移動します。</span><span class="sxs-lookup"><span data-stu-id="75398-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
