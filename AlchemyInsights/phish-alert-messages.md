---
title: "\"テナントまたはユーザーの上書きによって配信されたフィッシング\" ポリシーからのアラート メール メッセージ 2491"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544583"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="6c5d1-102">"テナントまたはユーザーの上書きによって配信されたフィッシング" ポリシーからのアラート メール メッセージ </span><span class="sxs-lookup"><span data-stu-id="6c5d1-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="6c5d1-103">"テナントまたはユーザーの上書きによって配信されたフィッシング" という名前の既定のアラート ポリシーは、Microsoft Defender for Office 365 P1 および P2 ライセンスのテナントに展開されています。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="6c5d1-104">このアラートを受け取った場合は、次の手順に従って調査してください。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="6c5d1-105">アラート メッセージで、[**アラートの表示**] をクリックし、セキュリティ/コンプライアンス センターの [**アラート**] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="6c5d1-106">アラートを選択し、[**メッセージ リストの表示**] または [**エクスプローラーでメッセージを表示**] を行うためのオプションを表示させます。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="6c5d1-107">いずれのオプションの場合でも、メッセージ ID などのメッセージの詳細情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="6c5d1-108">[脅威エクスプローラー] リンクでは、アラートの条件に一致するメッセージが自動的にフィルター処理されます。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="6c5d1-109">脅威エクスプローラーで日付フィルターの調整が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="6c5d1-110">手動で構成された上書きにより、フィッシング メッセージが送信されました:</span><span class="sxs-lookup"><span data-stu-id="6c5d1-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="6c5d1-111">ユーザーによって設定された、許可された送信者またはドメイン。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="6c5d1-112">迷惑メール対策ポリシーの管理者によって設定された、許可された送信者またはドメイン。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="6c5d1-113">接続フィルター ポリシーで許可されている IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="6c5d1-114">メッセージの受信を許可するように構成されたメール フロー ルール (トランスポート ルールとも呼ばれます)。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="6c5d1-115">メッセージが誤ってフィッシングとしてマークされていると思われる場合は、Outlook の[迷惑メール報告アドイン](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)を使用してメッセージのサンプルを Microsoft に送信してください。</span><span class="sxs-lookup"><span data-stu-id="6c5d1-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
