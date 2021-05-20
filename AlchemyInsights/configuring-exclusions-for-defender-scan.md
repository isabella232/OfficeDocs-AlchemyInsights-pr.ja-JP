---
title: Microsoft Defender ATP スキャンの除外の構成
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543690"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="03be4-102">Microsoft Defender ATP スキャンの除外の構成</span><span class="sxs-lookup"><span data-stu-id="03be4-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="03be4-103">一般に、特定のファイル拡張子とフォルダーの場所を Microsoft Defender ATP スキャンから除外できます。</span><span class="sxs-lookup"><span data-stu-id="03be4-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="03be4-104">特定のプロセスで開かれたファイルの除外も構成できます。</span><span class="sxs-lookup"><span data-stu-id="03be4-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="03be4-105">詳細については、「[ファイル拡張子とフォルダーの場所に基づく除外を構成し、検証する](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus)」と「[「プロセスによって開かれたファイルの除外を構成する](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="03be4-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="03be4-106">**Windows Server 2016 および 2019** 用の除外を構成するには、「[Windows Server で Microsoft Defender ウイルス対策を構成する](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="03be4-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="03be4-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="03be4-107">**Mac**</span></span>

<span data-ttu-id="03be4-108">Mac 用のサポートされている除外の種類と、除外リストを構成する方法の詳細については、「[サポートされている除外の種類](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)」と「[除外リストを構成する方法](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="03be4-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="03be4-109">**注** EICAR テスト ファイルを使用して、除外リストを検証することもできます。</span><span class="sxs-lookup"><span data-stu-id="03be4-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="03be4-110">詳細については、「[EICAR テスト ファイルを使用して除外リストを検証する](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="03be4-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="03be4-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="03be4-111">**Linux**</span></span>

<span data-ttu-id="03be4-112">Linux 用のサポートされている除外の種類と、 除外リストを構成する方法の詳細については、「[サポートされている除外の種類](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)」と、「[Linux 用の Microsoft Defender ATP の除外を構成し、検証する」](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="03be4-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="03be4-113">**注** EICAR テスト ファイルを使用して、除外リストを検証することもできます。</span><span class="sxs-lookup"><span data-stu-id="03be4-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="03be4-114">詳細については、「[EICAR テスト ファイルを使用して除外リストを検証する](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="03be4-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 