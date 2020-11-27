---
title: Microsoft Intune の Android アプリ保護ポリシーの設定
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
- "9003997"
- "7057"
ms.openlocfilehash: 327df6e0a901037cd929cb845f805466d9bd4eff
ms.sourcegitcommit: 81c86027933c06db08d264918f2698d9c9a1659a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2020
ms.locfileid: "49447602"
---
# <a name="android-app-protection-policy-settings-in-microsoft-intune"></a><span data-ttu-id="f9e06-102">Microsoft Intune の Android アプリ保護ポリシーの設定</span><span class="sxs-lookup"><span data-stu-id="f9e06-102">Android app protection policy settings in Microsoft Intune</span></span>

<span data-ttu-id="f9e06-103">Android デバイス用のアプリ保護ポリシーは 3 つのカテゴリに分類されます。</span><span class="sxs-lookup"><span data-stu-id="f9e06-103">There are three categories of app protection policy settings for Android devices:</span></span>

<span data-ttu-id="f9e06-104">**データ保護** は、データをコピーしたり、別のアプリケーションに貼り付けたり、アプリのスクリーンショットを撮影できるかどうかなど、会社のデータの処理方法を制御します。</span><span class="sxs-lookup"><span data-stu-id="f9e06-104">**Data protection** controls how company data is handled, such as, whether data can be copied or pasted to a different app or whether a screenshot can be taken of the app.</span></span> <span data-ttu-id="f9e06-105">この設定では、会社のデータに暗号化を適用したり、特定のデータを固有のデバイス アプリと同期できるかどうかを管理します (連絡先リスト、Web ブラウザーなど)。</span><span class="sxs-lookup"><span data-stu-id="f9e06-105">The settings also enforce encryption on company data and manage whether certain data can be synced with the native device apps, like the contact list or web browser.</span></span> <span data-ttu-id="f9e06-106">詳細については、「[データ保護](https://go.microsoft.com/fwlink/?linkid=2135259)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f9e06-106">To learn more, see [Data protection](https://go.microsoft.com/fwlink/?linkid=2135259).</span></span>

<span data-ttu-id="f9e06-107">**アクセス要件** は、アプリにユーザーがアクセスする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="f9e06-107">**Access requirements** guides how users can access an app.</span></span> <span data-ttu-id="f9e06-108">たとえば、アプリでは、アクセスするために PIN や指紋の入力が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f9e06-108">For example, an app could require the user to enter a PIN or fingerprint to access it.</span></span> <span data-ttu-id="f9e06-109">詳細については、「[アクセス要件](https://go.microsoft.com/fwlink/?linkid=2135260)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9e06-109">To learn more, see [Access requirements](https://go.microsoft.com/fwlink/?linkid=2135260).</span></span>

<span data-ttu-id="f9e06-110">**条件付き起動** は、アプリのサインイン セキュリティ設定を制御します。たとえば、ロックアウトの前に試みることができる最大限のPIN 入力回数や、アプリを実行するために必要な最小オペレーティング システムなどです。</span><span class="sxs-lookup"><span data-stu-id="f9e06-110">**Conditional launch** governs the sign-in security settings for an app, such as, the maximum PIN attempts before lockout or the minimum operating system needed to run the app.</span></span> <span data-ttu-id="f9e06-111">詳細については、「[条件付き起動](https://go.microsoft.com/fwlink/?linkid=2135507)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9e06-111">To learn more, see [Conditional launch](https://go.microsoft.com/fwlink/?linkid=2135507).</span></span>
