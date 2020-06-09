---
title: ライセンスのない製品というエラーを解決する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 89d0e589329d40f17c36baa54868154be0f5b887
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582744"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="e50d7-102">"ライセンスのない製品" エラーの解決方法の提案</span><span class="sxs-lookup"><span data-stu-id="e50d7-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="e50d7-103">"ライセンスのない製品" エラーを解決するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="e50d7-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="e50d7-104">サブスクリプション ステータスが期限切れになっていないかどうか確認します。</span><span class="sxs-lookup"><span data-stu-id="e50d7-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="e50d7-105">Microsoft 365 Apps for business や Business Premium など、クライアント ライセンスが許可されているサブスクリプションを持っていること、[ユーザーにライセンスが割り当てられていることを確認します](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。</span><span class="sxs-lookup"><span data-stu-id="e50d7-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="e50d7-106">ユーザーが、ライセンスが割り当てられているアカウントと同じアカウントで Office にサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e50d7-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="e50d7-107">[サービス正常性ページ](https://docs.microsoft.com/office365/enterprise/view-service-health)を確認し、サービスに既知の問題があるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="e50d7-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="e50d7-108">ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、Microsoft 365 アプリがインターネットにアクセスするのをそれらがブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="e50d7-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="e50d7-109">「 [URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e50d7-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="e50d7-110">また、トラブルシューティングのための次の操作を試すこともできます。</span><span class="sxs-lookup"><span data-stu-id="e50d7-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="e50d7-111">Office アプリを開き、既存のすべてのユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。</span><span class="sxs-lookup"><span data-stu-id="e50d7-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="e50d7-112">Office のライセンスを[削除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)して[再び割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)、影響を受けているユーザー アカウントを使用して [Office にサインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)します。</span><span class="sxs-lookup"><span data-stu-id="e50d7-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="e50d7-113">[ライセンス認証のトラブルシューティング ツール](https://aka.ms/SARA-OfficeActivation-Alchemy)を実行します。</span><span class="sxs-lookup"><span data-stu-id="e50d7-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="e50d7-114">[Office のライセンス認証の状態をリセットします](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)。</span><span class="sxs-lookup"><span data-stu-id="e50d7-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="e50d7-115">[Office のオンライン修復を実行します](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)。</span><span class="sxs-lookup"><span data-stu-id="e50d7-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="e50d7-116">その他のトラブルシューティングの手順については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e50d7-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="e50d7-117">Office でのライセンスのない製品というエラーとライセンス認証のエラー</span><span class="sxs-lookup"><span data-stu-id="e50d7-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="e50d7-118">Office のライセンス認証時の "申し訳ございません。お使いのアカウントに接続できません。後でもう一度やり直してください。" というエラー</span><span class="sxs-lookup"><span data-stu-id="e50d7-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)