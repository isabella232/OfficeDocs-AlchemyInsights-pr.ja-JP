---
title: Microsoft 365 経由の中継メール
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117988"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="dc4c9-102">多機能デバイスまたはアプリケーションを設定して、メールを送信します</span><span class="sxs-lookup"><span data-stu-id="dc4c9-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="dc4c9-103">オプションおよび手順の詳細については、「[多機能デバイスまたはアプリケーションを設定して、Microsoft 365 を使用してメールを送信する方法](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc4c9-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="dc4c9-104">最近動作を停止したデバイスまたはアプリケーションがある場合、最も一般的な問題は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="dc4c9-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="dc4c9-105">**SMTP 認証クライアント送信を使用時の認証関連エラー** 最近、SMTP 認証の動作に関連するいくつかの変更を行いました。</span><span class="sxs-lookup"><span data-stu-id="dc4c9-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="dc4c9-106">問題を解決する方法の詳細については、「[Microsoft 365 または Office 365 を使用して電子メールを送信するプリンター、スキャナー、および LOB アプリケーションの問題を修正する](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)」の「認証失敗」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc4c9-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="dc4c9-107">**Office 365 へのセキュリティで保護された接続を行っている間は TLS 1.2 バージョンのみを受け入れます** セキュリティで保護された接続 (TLS) を使用している場合は、アプリケーション デバイスで TLS 1.2 がサポートされていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="dc4c9-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="dc4c9-108">詳細については、「[Microsoft 365 および Office 365 GCC での TLS 1.2 の準備](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc4c9-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="dc4c9-109">その他の問題と解決策については、「[Microsoft 365 または Office 365 を使用して電子メールを送信するプリンター、スキャナー、および LOB アプリケーションの問題を解決する](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc4c9-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="dc4c9-110">影響を受けるデバイスを確認するには、「[SMTP Auth クライアントのレポート](https://protection.office.com/mailflow/dashboard)」に移動します。</span><span class="sxs-lookup"><span data-stu-id="dc4c9-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="dc4c9-p103">**注**: Exchange Online では、一括メールのシナリオには対応できません。一括商用メール (顧客ニュースレターなど) を送信するには、これらのサービスを専門とするサード パーティのプロバイダーを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc4c9-p103">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios. To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
