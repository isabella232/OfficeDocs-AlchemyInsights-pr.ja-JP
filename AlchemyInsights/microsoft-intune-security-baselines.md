---
title: Microsoft Intune セキュリティ ベースラインを使用して Windows 10 デバイスを構成する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794258"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="a1343-102">Microsoft Intune セキュリティ ベースラインを使用して Windows 10 デバイスを構成する</span><span class="sxs-lookup"><span data-stu-id="a1343-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="a1343-103">Intune セキュリティ ベースラインは、ユーザーとデバイスを保護するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a1343-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="a1343-104">セキュリティ ベースラインは事前構成済みの Windows 設定のグループで、関連するセキュリティ チームが推奨する一連の設定と既定値を適用するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="a1343-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="a1343-105">Intune でセキュリティ ベースラインのプロファイルを作成することで、複数のデバイス構成プロファイルで構成されたテンプレートを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1343-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="a1343-106">ユーザーやデバイスのグループに対してセキュリティ ベースラインを展開すると、Windows 10 以降を実行するデバイスに設定が適用されます。</span><span class="sxs-lookup"><span data-stu-id="a1343-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="a1343-107">たとえば、Microsoft モバイル デバイス管理 (MDM) セキュリティ ベースラインを使用すると、自動的にリムーバブル ドライブに対する BitLocker の有効化、デバイスのロックを解除するためのパスワードの要求、プレーンテキスト認証の無効化が実行されます。</span><span class="sxs-lookup"><span data-stu-id="a1343-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="a1343-108">既定値がご利用の環境でうまく機能しない場合には、ベースラインをカスタマイズして必要な設定を適用できます。</span><span class="sxs-lookup"><span data-stu-id="a1343-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="a1343-109">セキュリティ ベースラインは、セキュリティで保護されたエンド ツー エンドのワークフローを Microsoft 365 で確立するのにも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a1343-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="a1343-110">セキュリティ ベースラインには、セキュリティに影響を与える設定のベスト プラクティスとおすすめが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1343-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="a1343-111">Intune はグループ ポリシーのベースラインを作成する Windows セキュリティ チームと連携を図っているため、このようなおすすめは正確なガイダンスと豊富な経験に基づいています。</span><span class="sxs-lookup"><span data-stu-id="a1343-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="a1343-112">Intune を使用したことがなく、どこから手を付けたらよいか分からない場合、セキュリティ ベースラインはセキュリティで保護されたプロファイルをすばやく作成して展開するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a1343-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="a1343-113">セキュリティ ベースラインは Intune に組み込まれており、最先端の管理機能が含まれています。そのため、現在グループ ポリシーを使用している場合は、セキュリティ ベースラインを使用すると、管理目的で Intune に移行する作業がはるかに簡単になります。</span><span class="sxs-lookup"><span data-stu-id="a1343-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="a1343-114">詳細については、「[Windows セキュリティ ベースライン](/windows/security/threat-protection/windows-security-baselines)」および「[モバイル デバイス管理](/windows/client-management/mdm/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1343-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

