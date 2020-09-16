---
title: Office をライセンス認証することができない
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
- "2000023"
- "3509"
ms.openlocfilehash: 50939456df57920994e464db20e5da54f45f197a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744631"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="31d4c-102">Office をライセンス認証することができない</span><span class="sxs-lookup"><span data-stu-id="31d4c-102">Unable to activate Office</span></span>

- <span data-ttu-id="31d4c-103">サブスクリプションが期限切れの状態であるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="31d4c-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="31d4c-104">Office 365 Business や Business Premium など、クライアント ライセンスが許可されているサブスクリプションを持っていること、そして[ユーザーにライセンスが割り当てられていることを確認](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users)します。</span><span class="sxs-lookup"><span data-stu-id="31d4c-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="31d4c-105">ユーザーが、ライセンスが割り当てられているアカウントと同じアカウントで Office にサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="31d4c-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="31d4c-106">[Office 365 サービス正常性ページ](https://docs.microsoft.com/office365/enterprise/view-service-health)を確認し、サービスに既知の問題があるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="31d4c-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="31d4c-107">ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、Microsoft 365 アプリがインターネットにアクセスするのをそれらがブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="31d4c-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="31d4c-108">詳細については、「[Office 365 の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL および IP アドレス範囲")」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31d4c-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="31d4c-109">トラブルシューティングのための次の操作をお試しください。</span><span class="sxs-lookup"><span data-stu-id="31d4c-109">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="31d4c-110">Office アプリを開き、すべての既存のユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。</span><span class="sxs-lookup"><span data-stu-id="31d4c-110">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="31d4c-111">Office のライセンスを[削除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)して[再び割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)、影響を受けているユーザー アカウントを使用して [Office にサインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)します。</span><span class="sxs-lookup"><span data-stu-id="31d4c-111">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="31d4c-112">[ライセンス認証のトラブルシューティング ツール](https://aka.ms/SARA-OfficeActivation-Alchemy)を実行します。</span><span class="sxs-lookup"><span data-stu-id="31d4c-112">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- <span data-ttu-id="31d4c-113">[Office のライセンス認証の状態を再設定します](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office のライセンス認証の状態をリセットする")。</span><span class="sxs-lookup"><span data-stu-id="31d4c-113">[Reset Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reset Office activation state")</span></span>
- <span data-ttu-id="31d4c-114">[Office のオンライン修復を実行します](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)。</span><span class="sxs-lookup"><span data-stu-id="31d4c-114">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)</span></span>

<span data-ttu-id="31d4c-115">その他のトラブルシューティングの手順については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31d4c-115">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="31d4c-116">Office でのライセンスのない製品というエラーとライセンス認証のエラー</span><span class="sxs-lookup"><span data-stu-id="31d4c-116">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="31d4c-117">Office のライセンス認証時の "申し訳ございません。お使いのアカウントに接続できません。後でもう一度やり直してください。" というエラー</span><span class="sxs-lookup"><span data-stu-id="31d4c-117">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)