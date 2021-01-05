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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713513"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="8439e-102">Microsoft Defender ATP スキャンの除外の構成</span><span class="sxs-lookup"><span data-stu-id="8439e-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="8439e-103">一般に、特定のファイル拡張子とフォルダーの場所を Microsoft Defender ATP スキャンから除外できます。</span><span class="sxs-lookup"><span data-stu-id="8439e-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="8439e-104">特定のプロセスで開かれたファイルの除外も構成できます。</span><span class="sxs-lookup"><span data-stu-id="8439e-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="8439e-105">詳細については、「[ファイル拡張子とフォルダーの場所に基づく除外を構成し、検証する](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus)」と「[「プロセスによって開かれたファイルの除外を構成する](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8439e-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="8439e-106">**Windows Server 2016 および 2019** 用の除外を構成するには、「[Windows Server で Microsoft Defender ウイルス対策を構成する](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8439e-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="8439e-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="8439e-107">**Mac**</span></span>

<span data-ttu-id="8439e-108">Mac 用のサポートされている除外の種類と、除外リストを構成する方法の詳細については、「[サポートされている除外の種類](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)」と「[除外リストを構成する方法](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8439e-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="8439e-109">**注** EICAR テスト ファイルを使用して、除外リストを検証することもできます。</span><span class="sxs-lookup"><span data-stu-id="8439e-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="8439e-110">詳細については、「[EICAR テスト ファイルを使用して除外リストを検証する](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8439e-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="8439e-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="8439e-111">**Linux**</span></span>

<span data-ttu-id="8439e-112">Linux 用のサポートされている除外の種類と、 除外リストを構成する方法の詳細については、「[サポートされている除外の種類](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)」と、「[Linux 用の Microsoft Defender ATP の除外を構成し、検証する」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8439e-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="8439e-113">**注** EICAR テスト ファイルを使用して、除外リストを検証することもできます。</span><span class="sxs-lookup"><span data-stu-id="8439e-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="8439e-114">詳細については、「[EICAR テスト ファイルを使用して除外リストを検証する](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8439e-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 