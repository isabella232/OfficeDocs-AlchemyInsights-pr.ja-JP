---
title: プロビジョニング サービスの構成
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484183"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="a7077-102">プロビジョニング サービスの構成</span><span class="sxs-lookup"><span data-stu-id="a7077-102">Configuring the Provision service</span></span>

<span data-ttu-id="a7077-103">自動化されたユーザー プロビジョニングを機能させるには、Azure AD が Workday Web Services API に接続できるようにする有効な資格情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7077-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="a7077-104">さらに、Workday to AD ユーザーのプロビジョニング アプリの [接続テスト] ボタンは、AD ドメインに関連付けられた Azure AD Connect プロビジョニング エージェントに接続できるかどうかも検証します。</span><span class="sxs-lookup"><span data-stu-id="a7077-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="a7077-105">資格情報の保存時に Azure ポータルがエラーを返す場合は、以下の推奨手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="a7077-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="a7077-106">チュートリアル セクション「[Workday で統合システムユーザーを構成する](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)」の説明に従って、Workday 統合システム ユーザー アカウントを構成したことを確認します。</span><span class="sxs-lookup"><span data-stu-id="a7077-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="a7077-107">サービス管理コンソールを使用して、オンプレミスの Windows サーバーで Azure AD Connect プロビジョニング エージェント サービスが稼働していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a7077-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="a7077-108">[オンプレミス エージェントの表示] ボタンをクリックして、Azure ポータルでエージェントの状態を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="a7077-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="a7077-109">"Workday Username" フィールドの値を username@workday-tenant-name の形式で入力していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a7077-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="a7077-110">workday-tenant-name が欠落している場合、Workday 認証は失敗します。</span><span class="sxs-lookup"><span data-stu-id="a7077-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="a7077-111">Workday 実装テナントとの統合を構成している場合は、Workday テナントのスケジュールされたダウンタイム時間をメモしてください。</span><span class="sxs-lookup"><span data-stu-id="a7077-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="a7077-112">Workday は、週末 (通常は金曜日の夜から土曜日の朝) に実装テナントのダウンタイムをスケジュールしており、このダウンタイム ウィンドウ中の接続障害は、実装テナントがオンラインに戻るとすぐに自動解決される既知の問題です。</span><span class="sxs-lookup"><span data-stu-id="a7077-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="a7077-113">まれに、テナントの更新のために統合システム ユーザーのパスワードが変更された場合、またはアカウントがロック状態または期限切れ状態にある場合にも、このエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a7077-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="a7077-114">Integration System ユーザーのステータスを Workday 管理者に確認してください。</span><span class="sxs-lookup"><span data-stu-id="a7077-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="a7077-115">自動プロビジョニング用の Workday の構成の詳細については、「[チュートリアル: Workday を構成し、自動ユーザー プロビジョニングに対応させる](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7077-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
