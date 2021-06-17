---
title: Microsoft Intune を使用して、Microsoft Edge for iOS および Android での Web アクセスを管理する
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
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989678"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="009d0-102">Microsoft Intune を使用して、Microsoft Edge for iOS および Android での Web アクセスを管理する</span><span class="sxs-lookup"><span data-stu-id="009d0-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="009d0-103">Microsoft Edge for iOS および Android では、ユーザーは複数の完全に独立したプロファイルから Web をブラウズできます。</span><span class="sxs-lookup"><span data-stu-id="009d0-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="009d0-104">Microsoft Intune と Azure Active Directory Premium の機能を含む Enterprise Mobility + Security スイートに登録すると、条件付きアクセスなど、Microsoft 365 のデータの最も広範な保護機能を利用できます。</span><span class="sxs-lookup"><span data-stu-id="009d0-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="009d0-105">少なくとも、(1) ユーザーがモバイル デバイスから Microsoft Edge for iOS および Android に接続できるようにし、(2) 保護されたブラウジング エクスペリエンスを提供する Microsoft Intune のアプリ保護ポリシーを実装する条件付きアクセス ポリシーを展開する必要があります。</span><span class="sxs-lookup"><span data-stu-id="009d0-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="009d0-106">条件付きアクセスおよびポリシーの使用方法については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="009d0-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="009d0-107">Azure Active Directory の条件付きアクセス ポリシーを適用する</span><span class="sxs-lookup"><span data-stu-id="009d0-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="009d0-108">Microsoft Intune アプリ保護ポリシーを作成する</span><span class="sxs-lookup"><span data-stu-id="009d0-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="009d0-109">ポリシーで保護されたブラウザーで Azure Active Directory に接続された Web アプリにシングル サインオンを使用する</span><span class="sxs-lookup"><span data-stu-id="009d0-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="009d0-110">アプリの構成を使用して閲覧環境を管理する</span><span class="sxs-lookup"><span data-stu-id="009d0-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="009d0-111">職場と学校のアカウントのみの使用を許可する</span><span class="sxs-lookup"><span data-stu-id="009d0-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="009d0-112">一般的なアプリ構成ポリシーを展開する</span><span class="sxs-lookup"><span data-stu-id="009d0-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="009d0-113">データ保護のためのアプリ構成ポリシーを展開する</span><span class="sxs-lookup"><span data-stu-id="009d0-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="009d0-114">Microsoft エンドポイント マネージャー を使用してアプリ構成ポリシーを展開する</span><span class="sxs-lookup"><span data-stu-id="009d0-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="009d0-115">管理対象のアプリ ログへのアクセス方法については、「[Microsoft Edge for iOS および Android を使用して管理対象のアプリ ログにアクセスする](https://go.microsoft.com/fwlink/?linkid=2132578)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="009d0-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
