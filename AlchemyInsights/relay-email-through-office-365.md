---
title: Office 365 経由でメールを中継する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 9/21/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 84443cf1c93e9b19249c573704bc520eaa1c8f48
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36552981"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="6628a-102">Office 365 を使用してメールを送信するように多機能デバイスまたはアプリケーションをセットアップする</span><span class="sxs-lookup"><span data-stu-id="6628a-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="6628a-103">オプションと手順については、「[Office 365 を使用してメールを送信するように多機能デバイスまたはアプリケーションをセットアップする方法](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6628a-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="6628a-104">**注:** 最近動作しなくなったデバイスやアプリケーションがある場合、Microsoft は最近計画に従って [3DES 暗号の無効化](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption)を開始したことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6628a-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="6628a-105">影響を受けるデバイスを表示するには、「[SMTP Auth クライアントのレポート](https://protection.office.com/mailflow/dashboard)」に移動します。</span><span class="sxs-lookup"><span data-stu-id="6628a-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="6628a-106">一般的なエラーとしては、認証失敗/エラー、TLS 失敗/エラー、暗号アルゴリズム エラー、アルゴリズム不一致、接続の解除などがあります。</span><span class="sxs-lookup"><span data-stu-id="6628a-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="6628a-107">この問題を解決するには:</span><span class="sxs-lookup"><span data-stu-id="6628a-107">To resolve this issue:</span></span>
 - <span data-ttu-id="6628a-108">**Windows Server 2003 IIS SMTP は動作しなくなります。新しいバージョンの Windows が必要です。**</span><span class="sxs-lookup"><span data-stu-id="6628a-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="6628a-109">お使いのアプリケーションまたはデバイスの製造元に問い合わせて、最新の暗号がサポートされているかどうか、または更新プログラムがあるかどうかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="6628a-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
