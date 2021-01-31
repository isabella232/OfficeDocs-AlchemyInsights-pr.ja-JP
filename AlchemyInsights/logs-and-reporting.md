---
title: ログとレポーティング
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036134"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="5b0b4-102">ログとレポーティング</span><span class="sxs-lookup"><span data-stu-id="5b0b4-102">Logs and Reporting</span></span>

<span data-ttu-id="5b0b4-103">「[Azure Active Directory レポートに関する FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq)」では、Azure Active Directory (Azure AD) のレポート機能についてよく寄せられる質問への回答をご覧いただけます。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="5b0b4-104">レポートとレポートへのアクセス方法の詳細については、「[Azure Active Directory レポート](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="5b0b4-105">**監査に関する問題のトラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="5b0b4-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="5b0b4-106">監査アクティビティの一部が表示される問題が発生し、不足しているアクティビティがこの[リスト](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)に含まれている場合は、サポート チケットを提出してください。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="5b0b4-107">テナントで監査ログが表示される問題が発生している場合は、サポート チケットを提出してください。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="5b0b4-108">監査アクティビティがすぐに Azure portal に表示されない場合は「[遅延情報](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)」を確認し、遅延が記載されている遅延時間を超えている場合には、サポート チケットを提出してください。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="5b0b4-109">Azure AD アクティビティ ログの保持</span><span class="sxs-lookup"><span data-stu-id="5b0b4-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="5b0b4-110">選択した日付の範囲内のすべての監査が表示されない場合は、最大 25 万行 (最新のものから並べ替えて表示) のサインインを Azure portal からダウンロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="5b0b4-111">詳細については、「[Audit activities download (監査アクティビティのダウンロード)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="5b0b4-112">**サインインに関する問題のトラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="5b0b4-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="5b0b4-113">テナントの Azure AD Premium (P1 または P2) ライセンスを持っている場合のみ、過去 30 日間のデータを表示することができます。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="5b0b4-114">サインインは、Azure AD Premium のテナントのみで可能です。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="5b0b4-115">無料ライセンスまたは基本ライセンスのテナントではご利用いただけません。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="5b0b4-116">テナントに Premium P1 ライセンスをお持ちにもかかわらずサインインが表示されない場合は「[遅延情報](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)」を確認し、遅延が記載されている遅延時間を超えている場合には、サポート チケットを提出してください。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="5b0b4-117">選択した日付の範囲内のすべてのサインインが表示されない場合は、最大 25 万行 (最新のものから並べ替えて表示) のサインインを Azure portal からダウンロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="5b0b4-118">詳細については、「[Sign-ins activities download (サインイン アクティビティのダウンロード)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b0b4-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="5b0b4-119">**セキュリティ レポートのトラブルシューティング (危険、リスクの高いサインインのフラグが設定されているユーザー)**</span><span class="sxs-lookup"><span data-stu-id="5b0b4-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="5b0b4-120">リスク セキュリティ レポートのフラグが設定されたユーザー</span><span class="sxs-lookup"><span data-stu-id="5b0b4-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="5b0b4-121">Azure Active Directory ポータルのリスクの高いサインイン レポート</span><span class="sxs-lookup"><span data-stu-id="5b0b4-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="5b0b4-122">Azure Active Directory リスク イベント</span><span class="sxs-lookup"><span data-stu-id="5b0b4-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
