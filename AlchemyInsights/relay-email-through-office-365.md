---
title: Microsoft 365 経由の中継メール
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 180bae451941e4aaea94d285362794a797383eca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776491"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="63059-102">多機能デバイスまたはアプリケーションを設定して、メールを送信します</span><span class="sxs-lookup"><span data-stu-id="63059-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="63059-103">オプションおよび手順の詳細については、「[多機能デバイスまたはアプリケーションを設定して、Microsoft 365 を使用してメールを送信する方法](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63059-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="63059-104">**注:** 最近動作しなくなったデバイスやアプリケーションがある場合、Microsoft では最近、計画通りに[3DES 暗号の無効化](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption)を開始しましたので、ご留意ください。</span><span class="sxs-lookup"><span data-stu-id="63059-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="63059-105">影響を受けるデバイスを確認するには、「[SMTP Auth クライアントのレポート](https://protection.office.com/mailflow/dashboard)」に移動します。</span><span class="sxs-lookup"><span data-stu-id="63059-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="63059-106">一般的なエラーとしては、認証失敗/エラー、TLS 失敗/エラー、暗号アルゴリズム エラー、アルゴリズム不一致、接続の解除などがあります。</span><span class="sxs-lookup"><span data-stu-id="63059-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="63059-107">この問題を解決するには:</span><span class="sxs-lookup"><span data-stu-id="63059-107">To resolve the issue:</span></span>

 - <span data-ttu-id="63059-108">**Windows Server 2003 IIS SMTP は動作しなくなります。新しいバージョンの Windows が必要です。**</span><span class="sxs-lookup"><span data-stu-id="63059-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="63059-109">お使いのアプリケーションまたはデバイスの製造元に問い合わせて、最新の暗号がサポートされているかどうか、または更新プログラムがあるかどうかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="63059-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
