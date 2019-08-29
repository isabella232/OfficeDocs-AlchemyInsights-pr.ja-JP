---
title: Office 365 経由でメールを中継する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ffdaca1ba45a6f273809dbe50a7c40e8610193e1
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666521"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="f7c75-102">Office 365 を使用してメールを送信するように多機能デバイスまたはアプリケーションをセットアップする</span><span class="sxs-lookup"><span data-stu-id="f7c75-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="f7c75-103">オプションと手順については、「[Office 365 を使用してメールを送信するように多機能デバイスまたはアプリケーションをセットアップする方法](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7c75-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="f7c75-104">**注:** 最近動作しなくなったデバイスやアプリケーションがある場合、Microsoft では最近、計画通りに[3DES 暗号の無効化](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption)を開始しましたので、ご留意ください。</span><span class="sxs-lookup"><span data-stu-id="f7c75-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="f7c75-105">影響を受けるデバイスを確認するには、「[SMTP Auth クライアントのレポート](https://protection.office.com/mailflow/dashboard)」に移動します。</span><span class="sxs-lookup"><span data-stu-id="f7c75-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="f7c75-106">一般的なエラーとしては、認証失敗/エラー、TLS 失敗/エラー、暗号アルゴリズム エラー、アルゴリズム不一致、接続の解除などがあります。</span><span class="sxs-lookup"><span data-stu-id="f7c75-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="f7c75-107">この問題を解決するには:</span><span class="sxs-lookup"><span data-stu-id="f7c75-107">To resolve this issue:</span></span>
 - <span data-ttu-id="f7c75-108">**Windows Server 2003 IIS SMTP は動作しなくなります。新しいバージョンの Windows が必要です。**</span><span class="sxs-lookup"><span data-stu-id="f7c75-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="f7c75-109">お使いのアプリケーションまたはデバイスの製造元に問い合わせて、最新の暗号がサポートされているかどうか、または更新プログラムがあるかどうかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="f7c75-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
