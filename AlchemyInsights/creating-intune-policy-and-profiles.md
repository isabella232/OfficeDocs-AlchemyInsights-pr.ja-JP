---
title: Intune ポリシーとプロファイルを作成する
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 05/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: 580903fd89dca8a2ecbf635fa2157f31c93b85f4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363766"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="f4fd9-102">Intune ポリシーとプロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="f4fd9-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="f4fd9-103">Intune では、さまざまな事柄を実行するポリシーとプロファイルを作成できます。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="f4fd9-104">**登録プロファイル**: プラットフォームごとにデバイスを事前構成し、ユーザーアフィニティを有効にし、多要素認証を使用します。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="f4fd9-105">[デバイスの登録とは何ですか](https://docs.microsoft.com/intune/device-enrollment)。 [Android](https://docs.microsoft.com/intune/android-enroll)、 [IOS](https://docs.microsoft.com/intune/ios-enroll)、 [macOS](https://docs.microsoft.com/intune/macos-enroll)、および[Windows](https://docs.microsoft.com/intune/windows-enrollment-methods)の登録プロファイルを作成するのに適したリソースです。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="f4fd9-106">**コンプライアンスポリシー**: 準拠するためにデバイスが従う必要があるルールと設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="f4fd9-107">コンプライアンスポリシーを使用してデバイスを監視し、法令遵守ではないことをユーザーに通知することもできます。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="f4fd9-108">[デバイスコンプライアンスポリシー](https://docs.microsoft.com/intune/device-compliance-get-started)の概要を理解します。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="f4fd9-109">**条件付きアクセスポリシー**: 入力した条件に応じて、組織のリソースをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="f4fd9-110">たとえば、準拠していないデバイスでは、条件付きアクセスを使用して、電子メールと SharePoint へのアクセスを制限します。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="f4fd9-111">条件付きアクセスと、[条件付きアクセスを使用する一般的な方法](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use)[は](https://docs.microsoft.com/intune/conditional-access)、開始するのに適したリソースです。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="f4fd9-112">**構成プロファイル**: 電子メール設定、WiFi ネットワークの追加、組み込みテンプレートの使用、IOS および macOS デバイス機能の制御など、デバイス上の機能と設定を管理します。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="f4fd9-113">[デバイス構成プロファイル](https://docs.microsoft.com/intune/device-profiles)で作業を開始します。</span><span class="sxs-lookup"><span data-stu-id="f4fd9-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="f4fd9-114">役に立つリンク:</span><span class="sxs-lookup"><span data-stu-id="f4fd9-114">Helpful links:</span></span>

- [<span data-ttu-id="f4fd9-115">Intune でのデバイスポリシーとプロファイルに関する一般的な質問、問題、および解決策</span><span class="sxs-lookup"><span data-stu-id="f4fd9-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="f4fd9-116">Intune でのポリシーとプロファイルのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="f4fd9-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
