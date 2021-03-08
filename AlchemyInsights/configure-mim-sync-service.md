---
title: MIM 同期サービスを構成する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484062"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="d57a1-102">MIM 同期サービスを構成する</span><span class="sxs-lookup"><span data-stu-id="d57a1-102">Configure MIM Sync service</span></span>

<span data-ttu-id="d57a1-103">Microsoft Identity Manager (MIM) 同期サービスは MIM のコンポーネントです。</span><span class="sxs-lookup"><span data-stu-id="d57a1-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="d57a1-104">これは、複数のオンプレミス ディレクトリとデータベースを持つ組織の情報を保存および統合する一元化されたオンプレミス サービスです。</span><span class="sxs-lookup"><span data-stu-id="d57a1-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="d57a1-105">MIM の最近の更新で問題が解決された場合、または以下のセクションで説明されている他の問題の 1 つである場合は、MIM Sync の問題を解決できる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d57a1-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="d57a1-106">**推奨される手順**</span><span class="sxs-lookup"><span data-stu-id="d57a1-106">**Recommended steps**</span></span>

1. <span data-ttu-id="d57a1-107">MIM Sync の最新のアップデートを使用していることを確認し、[MIM Sync のリリース ノート](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history)を確認して、アップデートで問題が解決されたかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="d57a1-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="d57a1-108">問題が汎用 LDAP、汎用 SQL、Lotus Domino、または Web サービス コネクタにある場合は、[汎用コネクタ](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)の最新の更新を使用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="d57a1-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="d57a1-109">MIM 同期実行がエラーで停止した場合は、[実行エラーコード](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes)の表を参照して、考えられる原因を特定してください。</span><span class="sxs-lookup"><span data-stu-id="d57a1-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="d57a1-110">実行が **extension-dll-exception** で停止する場合は、それらの単語をクリックして **[コネクタ空間オブジェクト] プロパティ** ウィンドウを開き、**[スタック トレース...]** をクリックして、[Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) で説明されている根本的な原因の詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="d57a1-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="d57a1-111">パスワード変更通知サービス (PCNS) コンポーネントがパスワード同期中にイベント ログに **エラー 6025** を報告する場合は、[エラー 6025 を報告する PCNS](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx) のトラブルシューティング ガイドを確認してください。</span><span class="sxs-lookup"><span data-stu-id="d57a1-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="d57a1-112">FIM サービス管理エージェントとの完全同期が遅い場合は、「[遅いまたはハングする完全同期のトラブルシューティング](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)」で説明されているように、TempDB の **自動拡張** 設定を確認してください。</span><span class="sxs-lookup"><span data-stu-id="d57a1-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="d57a1-113">FIM サービス管理エージェントを使用して failed-creation-via-web-services で stopped-server のエラーが発生した場合は、原因の概要について、[Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d57a1-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

