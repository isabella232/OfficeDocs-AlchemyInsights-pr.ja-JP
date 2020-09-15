---
title: アプリケーションが検出されなかったエラーを軽減する
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
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666983"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="f5a3b-102">"アプリケーションが見つかりませんでした" というエラーを軽減する</span><span class="sxs-lookup"><span data-stu-id="f5a3b-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="f5a3b-103">Intune によって報告されたアプリ インストール エラー、 "インストールが正常に完了した後、アプリが検出されませんでした”は、すべての主要な OS プラットフォーム (Windows、iOS、Android) で発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="f5a3b-104">このエラーが発生する最も一般的なシナリオは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="f5a3b-105">初期展開後、アプリは Intune の外部(サードパーティのアプリストア)で更新されている場合。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="f5a3b-106">たとえば、Google Chrome などの一部のアプリケーションは、自動更新が実行される場合があります。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="f5a3b-107">ユーザーが、最初にインストールした後にアプリをアンインストールした場合。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="f5a3b-108">この問題を軽減するには、まず、影響を受けるデバイスを確認して、エラーが発生するシナリオを特定します。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="f5a3b-109">アプリが Intune 以外で更新されている場合は、アプリケーションのバージョンを無視するようにアプリの展開の設定ができます。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="f5a3b-110">この設定を行うには、**[アプリ構成] > [アプリの情報]** で、**[アプリのバージョンを無視]** を [**はい**] に設定します。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="f5a3b-111">クライアントを対象としている場合は、"必須" としてアプリケーションを展開して、最新バージョンが展開されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="f5a3b-112">または、iOS プラットフォームでは、Apple Volume Purchase Program に関連付けられている **autoupdate** 機能を使用できます。これは、新しいアプリケーション バージョンが利用可能になったときに自動的に更新されるように構成できます。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="f5a3b-113">アプリのインストールに関する問題のトラブルシューティングの詳細については、「[アプリのインストールの問題のトラブルシューティング](https://docs.microsoft.com/intune/troubleshoot-app-install)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5a3b-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
