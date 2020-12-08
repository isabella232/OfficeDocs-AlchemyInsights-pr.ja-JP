---
title: Microsoft Intune セキュリティ ベースラインを使用した Windows 10 デバイスの構成
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573944"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="b7f03-102">Microsoft Intune セキュリティ ベースラインを使用した Windows 10 デバイスの構成</span><span class="sxs-lookup"><span data-stu-id="b7f03-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="b7f03-103">Intune セキュリティ ベースラインは、ユーザーとデバイスを保護するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b7f03-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="b7f03-104">セキュリティ ベースラインは、関連するセキュリティ チームが推奨する設定のグループや既定値を適用するのに使用する、事前構成済みの Windows 設定のグループです。</span><span class="sxs-lookup"><span data-stu-id="b7f03-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="b7f03-105">Intune でセキュリティ ベースラインのプロファイルを作成することで、複数のデバイス構成プロファイルで構成されたテンプレートを作成します。</span><span class="sxs-lookup"><span data-stu-id="b7f03-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="b7f03-106">ユーザーやデバイスのグループに対してセキュリティ ベースラインを展開すると、Windows 10 以降を稼働するデバイスに設定が適用されます。</span><span class="sxs-lookup"><span data-stu-id="b7f03-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="b7f03-107">たとえば、MDM セキュリティ ベースラインを使用すると、自動的に (1) リムーバブル ドライブに対する BitLocker の有効化、(2) デバイスのロックを解除するためのパスワードの要求、(3) 基本認証の無効化が実行されます。</span><span class="sxs-lookup"><span data-stu-id="b7f03-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="b7f03-108">既定値がご利用の環境でうまく機能しない場合は、必要な設定が適用されるようベースラインをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="b7f03-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="b7f03-109">セキュリティ ベースラインは、Microsoft 365 でエンド ツー エンドのセキュリティで保護されたワークフローを確立するのにも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b7f03-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="b7f03-110">これには次のような利点があります。</span><span class="sxs-lookup"><span data-stu-id="b7f03-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="b7f03-111">セキュリティ ベースラインには、セキュリティに影響を与える設定のベスト プラクティスとおすすめが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7f03-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="b7f03-112">Intune はグループ ポリシーのベースラインを作成する Windows セキュリティ チームとパートナー関係を結んでいるため、このようなおすすめは正確なガイダンスと豊富な経験に基づいています。</span><span class="sxs-lookup"><span data-stu-id="b7f03-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="b7f03-113">Intune を使用したことがなく、どこから手を付けたらよいか分からない場合、セキュリティ ベースラインはセキュリティで保護されたプロファイルをすばやく作成して展開するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b7f03-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="b7f03-114">セキュリティ ベースラインは Intune に組み込まれており、管理に使用できる最先端の機能が含まれています。そのため、現在グループ ポリシーを使用している場合は、セキュリティ ベースラインを使用すると、管理目的で Intune に移行する作業がはるかに簡単になります。</span><span class="sxs-lookup"><span data-stu-id="b7f03-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="b7f03-115">詳細については、「[Windows セキュリティ ベースライン](https://go.microsoft.com/fwlink/?linkid=2141503)」と「[モバイル デバイス管理](https://go.microsoft.com/fwlink/?linkid=2141701)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7f03-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>