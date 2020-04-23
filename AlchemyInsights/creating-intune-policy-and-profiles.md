---
title: Intune ポリシーおよびプロフィールを作成する
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: fac2a9e41449b4eb9b87d21d4cba4f6f5192d9c6
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715401"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="8e83d-102">Intune ポリシーおよびプロフィールの作成</span><span class="sxs-lookup"><span data-stu-id="8e83d-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="8e83d-103">Intune では、異なる使用目的のためにポリシーおよびプロファイルを作成できます。</span><span class="sxs-lookup"><span data-stu-id="8e83d-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="8e83d-104">**登録プロファイル**: プラットフォーム別のデバイスの事前構成、ユーザー アフィニティの有効化、多要素認証の使用など。</span><span class="sxs-lookup"><span data-stu-id="8e83d-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="8e83d-105">「[デバイス登録とは](https://docs.microsoft.com/intune/device-enrollment)」ならびに [Android](https://docs.microsoft.com/intune/android-enroll)、[iOS](https://docs.microsoft.com/intune/ios-enroll)、[macOS](https://docs.microsoft.com/intune/macos-enroll)、および [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) での登録プロファイルに関する記事で、役立つリソースが提供されています。</span><span class="sxs-lookup"><span data-stu-id="8e83d-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="8e83d-106">**コンプライアン スポリシー**: 準拠するために必要なデバイスのルールと設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="8e83d-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="8e83d-107">また、コンプライアンス ポリシーを使用してデバイスを監視し、コンプライアンス違反をユーザーに通知することもできます。</span><span class="sxs-lookup"><span data-stu-id="8e83d-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="8e83d-108">[デバイス コンプライアンス ポリシー](https://docs.microsoft.com/intune/device-compliance-get-started)の概要に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8e83d-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="8e83d-109">**条件付きアクセス ポリシー**: 入力した条件に応じて、組織のリソースを保護します。</span><span class="sxs-lookup"><span data-stu-id="8e83d-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="8e83d-110">たとえば、準拠していないデバイスでは、条件付きアクセスを使用してメールや SharePoint へのアクセスを制限できます。</span><span class="sxs-lookup"><span data-stu-id="8e83d-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="8e83d-111">使用を開始するのに役立つリソースが「[条件付きアクセスとは](https://docs.microsoft.com/intune/conditional-access)」および「[Intune での条件付きアクセスの一般的な使用方法](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use)」で提供されています。</span><span class="sxs-lookup"><span data-stu-id="8e83d-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="8e83d-112">**構成プロファイル**: デバイスの機能と設定を管理します。これには、メールの設定、Wi-Fi ネットワークの追加、組み込みのテンプレートの使用、iOS や macOS デバイス機能の使用などが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8e83d-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="8e83d-113">使用を開始するには、[バイス構成プロファイル](https://docs.microsoft.com/intune/device-profiles)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8e83d-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="8e83d-114">便利なリンク:</span><span class="sxs-lookup"><span data-stu-id="8e83d-114">Helpful links:</span></span>

- [<span data-ttu-id="8e83d-115">Microsoft Intune でのデバイス ポリシーとプロファイルの一般的な質問、問題と解決策</span><span class="sxs-lookup"><span data-stu-id="8e83d-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="8e83d-116">Intune でのポリシーとプロファイルのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="8e83d-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
