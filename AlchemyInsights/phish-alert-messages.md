---
title: 2491テナントまたはユーザーの上書きにより配信された "フィッシングからの電子メールメッセージの通知" ポリシー
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36397240"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="e0223-102">[テナントまたはユーザーの上書きによって配信されたフィッシング] ポリシーから電子メールメッセージを通知する</span><span class="sxs-lookup"><span data-stu-id="e0223-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="e0223-103">「テナントまたはユーザーの上書きによって配信されたフィッシング」という名前の既定の通知ポリシーが、Office 365 ATP P1 および P2 ライセンスを使用してテナントにロールアウトされています。</span><span class="sxs-lookup"><span data-stu-id="e0223-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="e0223-104">この通知を受信した場合は、次の手順を使用して調査する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0223-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="e0223-105">通知メッセージで、[**警告の表示**] をクリックして、セキュリティ & コンプライアンスセンターの [**通知**] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="e0223-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="e0223-106">通知を選択して、エクスプローラーで**メッセージリストを表示**したり、**メッセージを表示**したりするオプションを表示します。</span><span class="sxs-lookup"><span data-stu-id="e0223-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="e0223-107">どちらのオプションでも、メッセージの ID が含まれているメッセージの詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="e0223-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="e0223-108">脅威エクスプローラーのリンクによって、通知の条件に一致するメッセージが自動的にフィルター処理されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="e0223-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="e0223-109">脅威エクスプローラーで日付フィルターを調整する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="e0223-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="e0223-110">手動で構成された上書きが原因で、フィッシングメッセージが配信されました。</span><span class="sxs-lookup"><span data-stu-id="e0223-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="e0223-111">許可された送信者またはドメインがユーザーによって設定されている。</span><span class="sxs-lookup"><span data-stu-id="e0223-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="e0223-112">スパム対策ポリシーで、管理者によって設定された送信者またはドメインの許可。</span><span class="sxs-lookup"><span data-stu-id="e0223-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="e0223-113">接続フィルターポリシーで許可されている IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="e0223-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="e0223-114">でメッセージを許可するように構成されたメールフロールール (トランスポートルールとも呼ばれます)。</span><span class="sxs-lookup"><span data-stu-id="e0223-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="e0223-115">メッセージが誤ってフィッシングとしてマークされていると思われる場合は、Outlook[レポートメッセージアドイン](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)を使用して、メッセージサンプルを Microsoft に送信します。</span><span class="sxs-lookup"><span data-stu-id="e0223-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
