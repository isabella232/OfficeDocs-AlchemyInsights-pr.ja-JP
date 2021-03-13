---
title: Microsoft Intune セキュリティ ベースラインを使用して Windows 10 デバイスを構成する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696554"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="4713f-102">Windows 10 デバイスの構成に Microsoft Intune セキュリティ ベースラインを使用する</span><span class="sxs-lookup"><span data-stu-id="4713f-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="4713f-103">Intune セキュリティ ベースラインは、ユーザーとデバイスを保護するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4713f-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="4713f-104">セキュリティ ベースラインは事前構成済みの Windows 設定のグループで、関連するセキュリティ チームが推奨する一連の設定と既定値を適用するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="4713f-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="4713f-105">Intune でセキュリティ ベースラインのプロファイルを作成することで、複数のデバイス構成プロファイルで構成されたテンプレートを作成します。</span><span class="sxs-lookup"><span data-stu-id="4713f-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="4713f-106">ユーザーやデバイスのグループに対してセキュリティ ベースラインを展開すると、Windows 10 以降のバージョンを実行しているデバイスに設定が適用されます。</span><span class="sxs-lookup"><span data-stu-id="4713f-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="4713f-107">たとえば、Microsoft モバイル デバイス管理 (MDM) セキュリティ ベースラインを使用すると、自動的に (1) リムーバブル ドライブに対する BitLocker の有効化、(2) デバイスのロックを解除するためのパスワードの要求、(3) プレーンテキスト認証の無効化が実行されます。</span><span class="sxs-lookup"><span data-stu-id="4713f-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="4713f-108">既定値がご利用の環境でうまく機能しない場合には、ベースラインをカスタマイズして必要な設定を適用できます。</span><span class="sxs-lookup"><span data-stu-id="4713f-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="4713f-109">セキュリティ ベースラインは、セキュリティで保護されたエンド ツー エンドのワークフローを Microsoft 365 で確立するのにも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4713f-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="4713f-110">この機能には、次のような利点があります。</span><span class="sxs-lookup"><span data-stu-id="4713f-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="4713f-111">セキュリティ ベースラインには、セキュリティに影響を与える設定のベスト プラクティスとおすすめが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4713f-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="4713f-112">Intune はグループ ポリシーのベースラインを作成する Windows セキュリティ チームと連携を図っているため、このようなおすすめは正確なガイダンスと豊富な経験に基づいています。</span><span class="sxs-lookup"><span data-stu-id="4713f-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="4713f-113">Intune を使用したことがなく、どこから手を付けたらよいか分からない場合、セキュリティ ベースラインはセキュリティで保護されたプロファイルをすばやく作成して展開するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4713f-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="4713f-114">これらのセキュリティ ベースラインは Intune に組み込まれており、管理に使用できる最先端の機能が含まれています。そのため、現在グループ ポリシーを使用している場合には、セキュリティ ベースラインを使用すると、管理目的で Intune に移行する作業がはるかに簡単になります。</span><span class="sxs-lookup"><span data-stu-id="4713f-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="4713f-115">詳細については、「[Windows セキュリティ ベースライン](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines)」および「[モバイル デバイス管理](https://docs.microsoft.com/windows/client-management/mdm/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4713f-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>