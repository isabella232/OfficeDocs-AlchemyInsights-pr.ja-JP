---
title: パスワード ログ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527960"
---
# <a name="password-logs"></a><span data-ttu-id="ae536-102">パスワード ログ</span><span class="sxs-lookup"><span data-stu-id="ae536-102">Password logs</span></span>

<span data-ttu-id="ae536-103">**パスワード リセットの監査ログへのアクセスに問題が発生しています**。</span><span class="sxs-lookup"><span data-stu-id="ae536-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="ae536-104">パスワード リセット監査ログへのアクセスに関する問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="ae536-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="ae536-105">監査ログを表示する権限があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ae536-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="ae536-106">次のロールのみ認証されています。</span><span class="sxs-lookup"><span data-stu-id="ae536-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="ae536-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="ae536-107">Global administrator</span></span>
 - <span data-ttu-id="ae536-108">セキュリティ管理者</span><span class="sxs-lookup"><span data-stu-id="ae536-108">Security administrator</span></span>
 - <span data-ttu-id="ae536-109">セキュリティ閲覧者</span><span class="sxs-lookup"><span data-stu-id="ae536-109">Security reader</span></span>

<span data-ttu-id="ae536-110">**最初に展開したときからのすべてのパスワード リセット監査イベントを確認したい**</span><span class="sxs-lookup"><span data-stu-id="ae536-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="ae536-111">過去 30 日間のレポートには、最大 12 万件のパスワード リセット/登録イベントが保存されています。</span><span class="sxs-lookup"><span data-stu-id="ae536-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="ae536-112">この上限は CSV をダウンロードする場合の UI に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ae536-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="ae536-113">100 万件のイベントが PowerShell から利用可能です。</span><span class="sxs-lookup"><span data-stu-id="ae536-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="ae536-114">詳細については、以下のリンクを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae536-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="ae536-115">Azure AD Reports and Events API でのセルフサービスのパスワード リセット イベント</span><span class="sxs-lookup"><span data-stu-id="ae536-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ae536-116">PowerShell を使用してパスワード リセット登録イベントを素早くダウンロードする方法</span><span class="sxs-lookup"><span data-stu-id="ae536-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="ae536-117">**パスワード リセットのレポート機能について詳しく知りたい**</span><span class="sxs-lookup"><span data-stu-id="ae536-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="ae536-118">Azure ポータルの **[ユーザーとグループ]** の Azure AD パスワード リセット監査ログで、登録しているユーザーやパスワードをリセットしているユーザーを確認します。</span><span class="sxs-lookup"><span data-stu-id="ae536-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="ae536-119">詳細については、以下のリンクを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae536-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="ae536-120">パスワード リセット レポートの概要</span><span class="sxs-lookup"><span data-stu-id="ae536-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ae536-121">Azure ポータルでパスワード リセット レポートを表示する方法</span><span class="sxs-lookup"><span data-stu-id="ae536-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ae536-122">Azure AD Reports and Events API でのセルフサービスのパスワード リセット イベント</span><span class="sxs-lookup"><span data-stu-id="ae536-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ae536-123">PowerShell を使用してパスワード リセット登録イベントを素早くダウンロードする方法</span><span class="sxs-lookup"><span data-stu-id="ae536-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


