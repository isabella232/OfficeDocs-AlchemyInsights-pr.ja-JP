---
title: Office をライセンス認証することができない
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798685"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="c8bfe-102">Office をライセンス認証することができない</span><span class="sxs-lookup"><span data-stu-id="c8bfe-102">Unable to activate Office</span></span>

<span data-ttu-id="c8bfe-103">**注**: 以前のバージョンの Windows (Windows 7 など) を使用している場合は、TLS 1.2 が既定で有効になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="c8bfe-104">詳細については、「[Windows の WinHTTP で TLS 1.1 および TLS 1.2 を既定のセキュリティ で保護されたプロトコルとして有効にするための更新プログラム](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="c8bfe-105">サブスクリプションが期限切れの状態であるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="c8bfe-106">Office 365 Business や Business Premium など、クライアント ライセンスが許可されているサブスクリプションを持っていること、そして[ユーザーにライセンスが割り当てられていることを確認](/microsoft-365/admin/manage/assign-licenses-to-users)します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="c8bfe-107">ユーザーが、ライセンスが割り当てられているアカウントと同じアカウントで Office にサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="c8bfe-108">[Office 365 サービス正常性ページ](/office365/enterprise/view-service-health)を確認し、サービスに既知の問題があるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="c8bfe-109">ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、Microsoft 365 アプリがインターネットにアクセスするのをそれらがブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="c8bfe-110">詳細については、「[Office 365 の URL と IP アドレスの範囲](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL および IP アドレス範囲")」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="c8bfe-111">Windows コンピューターについての **ヒント**、Office の一般的なサインインの問題を診断して、自動的に修正することができます。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="c8bfe-112">**[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA-OfficeSignInScenario)** をダウンロードして実行し、自動化ツールを使用します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="c8bfe-113">トラブルシューティングのための次の操作をお試しください。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="c8bfe-114">Office アプリを開き、すべての既存のユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="c8bfe-115">Office のライセンスを[削除](/microsoft-365/admin/manage/remove-licenses-from-users)して[再び割り当て](/microsoft-365/admin/manage/assign-licenses-to-users)、影響を受けているユーザー アカウントを使用して [Office にサインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="c8bfe-116">[ライセンス認証のトラブルシューティング ツール](https://aka.ms/SARA-OfficeActivation-Alchemy)を実行します。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- <span data-ttu-id="c8bfe-117">[Office のライセンス認証の状態を再設定します](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office のライセンス認証の状態をリセットする")。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-117">[Reset Office activation state](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reset Office activation state")</span></span>
- <span data-ttu-id="c8bfe-118">[Office のオンライン修復を実行します](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-118">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)</span></span>

<span data-ttu-id="c8bfe-119">その他のトラブルシューティングの手順については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8bfe-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="c8bfe-120">Office でのライセンスのない製品というエラーとライセンス認証のエラー</span><span class="sxs-lookup"><span data-stu-id="c8bfe-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="c8bfe-121">Office のライセンス認証時の "申し訳ございません。お使いのアカウントに接続できません。後でもう一度やり直してください。" というエラー</span><span class="sxs-lookup"><span data-stu-id="c8bfe-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)