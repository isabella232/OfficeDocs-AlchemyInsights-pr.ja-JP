---
title: パスワードの書き戻しが機能しません
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243789"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="0c9b1-102">パスワードの書き戻しが機能しません</span><span class="sxs-lookup"><span data-stu-id="0c9b1-102">Password Writeback is not working</span></span>

<span data-ttu-id="0c9b1-103">**パスワードの書き戻しの設定に問題があります**</span><span class="sxs-lookup"><span data-stu-id="0c9b1-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="0c9b1-104">パスワードの書き戻しはプレミアム機能です。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="0c9b1-105">ライセンス要件を理解していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="0c9b1-106">組織内で少なくとも 1 つのライセンスが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="0c9b1-107">**クラウド専用ユーザー** - 任意の Office 365 (O365) 有料 SKU または Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="0c9b1-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="0c9b1-108">**クラウドとオンプレミス ユーザー** - Azure AD Premium P1 または P2、Enterprise Mobility + Security (EMS)、または Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="0c9b1-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="0c9b1-109">ライセンス要件の詳細については、「[Azure AD セルフサービスによるパスワードのリセットのライセンス要件](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="0c9b1-110">適切なライセンスの 1 つを持つ、少なくとも 1 つの管理者アカウントと 1 つのテスト ユーザー アカウントがあります。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="0c9b1-111">パスワードの書き戻しを機能させるには、Azure AD Connect をプライマリ ドメイン コントローラーのエミュレーターに接続する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="0c9b1-112">Active Directory 同期コネクタの **[プロパティ]** を右クリックし、**[ディレクトリ パーティションを構成する]** を選択することで、プライマリ ドメイン コントローラーを使用するように Azure AD Connect を構成できます。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="0c9b1-113">そこから、**[ドメイン コントローラーの接続設定]** セクションを探し、**[優先ドメイン コントローラーのみを使用する]** というタイトルのチェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="0c9b1-114">優先 DC が PDC エミュレーターでない場合でも、Azure AD Connect はパスワードの書き戻しのために PDC に連絡します。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="0c9b1-115">テナントでパスワードのリセットが構成され、有効になっています。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="0c9b1-116">詳細については、「[ユーザーが Azure AD パスワードをリセットできるようにする](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="0c9b1-117">パスワードの書き戻しを有効にするために使用されている管理者アカウントがクラウド管理者アカウントであることを確認してください (オンプレミス AD ではなく Azure AD で作成されます)</span><span class="sxs-lookup"><span data-stu-id="0c9b1-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="0c9b1-118">Windows Server 2008 R2、Windows Server 2012、または最新のサービスパックがインストールされた Windows Server 2012 R2 を実行しているシングルまたはマルチフォレスト AD オンプレミス展開があります</span><span class="sxs-lookup"><span data-stu-id="0c9b1-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="0c9b1-119">Azure AD Connect ツールがインストールされており、クラウドと同期するための AD 環境が準備されています。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="0c9b1-120">パスワードの書き戻しをテストする前に、Azure AD Connect で AD と Azure AD の両方から完全なインポートと完全な同期を完了していることを最初に確認してください。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="0c9b1-121">詳細については、「[Azure AD Connect での完全同期と完全インポート](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="0c9b1-122">**パスワードの書き戻し接続に問題があります**</span><span class="sxs-lookup"><span data-stu-id="0c9b1-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="0c9b1-123">最新バージョンの [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594) をダウンロードして有効にします</span><span class="sxs-lookup"><span data-stu-id="0c9b1-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="0c9b1-124">ファイアウォール構成: Azure AD Connect ツール (1.1.443 以降) には、以下への **アウトバウンド HTTPS** アクセスが必要です。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="0c9b1-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0c9b1-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="0c9b1-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="0c9b1-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="0c9b1-127">アイドル状態の接続を、少なくとも 2-3 分間持続させます</span><span class="sxs-lookup"><span data-stu-id="0c9b1-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="0c9b1-128">**パスワードの書き戻しにまだ問題があります**</span><span class="sxs-lookup"><span data-stu-id="0c9b1-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="0c9b1-129">それでも問題が解決しない場合は、Azure AD Connect ツールで パスワードの書き戻しサービスを無効にしてから再度有効にしてみてください</span><span class="sxs-lookup"><span data-stu-id="0c9b1-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="0c9b1-130">詳細については、[パスワードの書き戻しを無効にしてから再度有効にする](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)方法をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0c9b1-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
