---
title: 1385-Office-365-アラート-ポリシー
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 1209e59668bbe69fe88408933ae11b357b8d4f1a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687623"
---
# <a name="alert-policies"></a><span data-ttu-id="af464-102">ポリシーを通知する</span><span class="sxs-lookup"><span data-stu-id="af464-102">Alert policies</span></span>

<span data-ttu-id="af464-p101">Microsoft 365 セキュリティ & コンプライアンスセンターでは、Office 365 Enterprise または Office 365 の米国政府 E1/G1、E3/G3、または E5/G5 サブスクリプションを使用して組織に対する通知をトリガーする[既定の通知ポリシー](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies)が提供されます。したがって、管理者は、Office365Alerts@microsoft.com によって送信された通知電子メール通知を、"低重要度アラート:*警告ポリシーの名前*" のような件名で受信することがあります。アラート通知は、次のような一般的なアクティビティに対してアラートがトリガーされたときに送信されます。</span><span class="sxs-lookup"><span data-stu-id="af464-p101">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription. Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*". Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="af464-106">メールを転送する受信トレイのルールを作成する。</span><span class="sxs-lookup"><span data-stu-id="af464-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="af464-107">アクセス許可をメールボックスに割り当てる。</span><span class="sxs-lookup"><span data-stu-id="af464-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="af464-108">SharePoint ファイル共有で、多数のファイルを共有または削除します。</span><span class="sxs-lookup"><span data-stu-id="af464-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="af464-109">電子情報開示検索を実行し、検索結果をエクスポートする。</span><span class="sxs-lookup"><span data-stu-id="af464-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="af464-110">アラートを確認して対応するには、次の操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="af464-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="af464-111">[セキュリティ/コンプライアンス センター](https://protection.office.com)に移動して、サインインします。</span><span class="sxs-lookup"><span data-stu-id="af464-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="af464-112">[**アラート**] >  [**アラートの表示**] の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="af464-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="af464-113">アラートをクリックして、アラートに関する情報を含むポップアップ ページを表示させます。</span><span class="sxs-lookup"><span data-stu-id="af464-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="af464-p102">アラートに対して、[不審な受信トレイのルールの削除](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account)などの操作を実行することができます。または、単にアラートのポップアップ ページで **[解決]** をクリックして、アラートを閉じることもできます。</span><span class="sxs-lookup"><span data-stu-id="af464-p102">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account). Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="af464-116">アラート ポリシーの構成と管理の詳細については、[こちらの記事](https://docs.microsoft.com/office365/securitycompliance/alert-policies)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af464-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>

<span data-ttu-id="af464-117">**重要**: Microsoft からのアラートのメール通知では、次の操作を要求することは決してありません。</span><span class="sxs-lookup"><span data-stu-id="af464-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="af464-118">パスワードを入力する</span><span class="sxs-lookup"><span data-stu-id="af464-118">Provide a password</span></span>
- <span data-ttu-id="af464-119">アカウントのセキュリティについての詳細を確認する</span><span class="sxs-lookup"><span data-stu-id="af464-119">Verify the security details of your account</span></span>
- <span data-ttu-id="af464-120">自分自身を再認証する</span><span class="sxs-lookup"><span data-stu-id="af464-120">Re-authenticate yourself</span></span>

<span data-ttu-id="af464-p103">このようなメール メッセージを受信した場合、Microsoft から送信されたものではありませんので、フィッシング詐欺を疑ってください。そうしたメールを受け取ったら、[Microsoft に報告してください](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)。</span><span class="sxs-lookup"><span data-stu-id="af464-p103">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam. If that happens, please [report it to Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>