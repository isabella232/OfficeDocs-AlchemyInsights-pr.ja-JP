---
title: Microsoft 365 アプリへのサインインに関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836608"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="de1ae-102">Microsoft 365 アプリへのサインインに関する問題</span><span class="sxs-lookup"><span data-stu-id="de1ae-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="de1ae-103">Microsoft 365 アプリに関するサインインの問題を修正するには、問題が発生しているコンピューターで次のオプションを試してみてください。</span><span class="sxs-lookup"><span data-stu-id="de1ae-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="de1ae-104">Windows の場合は、「[Recommendations on resolving common sign-in issues (サインインに関する一般的な問題の解決についての推奨事項)](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)」を参照してください</span><span class="sxs-lookup"><span data-stu-id="de1ae-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="de1ae-105">Mac の場合は、「[Office 2016 for Mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください</span><span class="sxs-lookup"><span data-stu-id="de1ae-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="de1ae-106">Windows コンピューターについての **ヒント**、Office の一般的なサインインの問題を診断して、自動的に修正することができます。</span><span class="sxs-lookup"><span data-stu-id="de1ae-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="de1ae-107">**[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA-OfficeSignInScenario)** をダウンロードして実行し、自動化ツールを使用します。</span><span class="sxs-lookup"><span data-stu-id="de1ae-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="de1ae-108">**注:** サインインやアクティベーションの問題を解決するために先進認証 (ADAL) や Web アカウント管理 (WAM) を無効にすることは、**推奨されていません**。</span><span class="sxs-lookup"><span data-stu-id="de1ae-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="de1ae-109">Office 2013 を使用し Microsoft 365 へと接続する際にエラーが発生した場合は、Office クライアントの[先進認証が有効](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="de1ae-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="de1ae-110">具体的なトラブルシューティングの手順については、以下をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="de1ae-110">For specific troubleshooting actions, see:</span></span>

<span data-ttu-id="de1ae-111">「[Windows 10 の Office 2016 ビルド16.0.7967 に更新後のサインインにおける接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」</span><span class="sxs-lookup"><span data-stu-id="de1ae-111">[Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span></span>  

<span data-ttu-id="de1ae-112">「[You can't sign in to your organizational account such as Office 365, Azure, or Intune (Office 365、Azure、Intune などの組織アカウントにサインインできない)](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)」</span><span class="sxs-lookup"><span data-stu-id="de1ae-112">[You can't sign in to your organizational account such as Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)</span></span>

<span data-ttu-id="de1ae-113">「[How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune (Office 365、Azure、または Intune にサインインできない非ブラウザー アプリのトラブルシューティング)](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)」</span><span class="sxs-lookup"><span data-stu-id="de1ae-113">[How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)</span></span>

<span data-ttu-id="de1ae-114">「[Repeatedly prompted for credentials in Office (Office で資格情報を繰り返し要求される)](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)」</span><span class="sxs-lookup"><span data-stu-id="de1ae-114">[Repeatedly prompted for credentials in Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)</span></span>