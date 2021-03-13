---
title: 例となる Microsoft Defender for Office 365 フィッシング対策ポリシーはありません。
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751432"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="053e9-102">例となる Microsoft Defender for Office 365 フィッシング対策ポリシーはありません。</span><span class="sxs-lookup"><span data-stu-id="053e9-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="053e9-103">これらの設定により、「*ドメインおよびCEO*」と呼ばれるポリシーが有効になります。</span><span class="sxs-lookup"><span data-stu-id="053e9-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="053e9-104">このポリシーは、ユーザーとドメインの両方を偽装から保護し、ドメイン内のユーザーが受信するメールにポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="053e9-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="053e9-105">最初に、パッケージを作成するために、次の情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="053e9-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="053e9-106">**名前**: ドメインと CEO の **説明**: CEO とお客様のドメインが偽装されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="053e9-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="053e9-107">**適用となる対象**: [**受信者のドメインは**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="053e9-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="053e9-108">[**これらの内のいずれか**] で、[**選択**] を選択し、それからドメインを選択します。</span><span class="sxs-lookup"><span data-stu-id="053e9-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="053e9-109">**[+ 追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="053e9-109">Select **+ Add**.</span></span> <span data-ttu-id="053e9-110">リスト内のドメイン名(*contoso.com* など)の横にあるチェックボックスを選択し、[**追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="053e9-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="053e9-111">[**完了**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="053e9-111">Select **Done**.</span></span>
- <span data-ttu-id="053e9-112">ポリシーを作成したら、次のオプションを使用してポリシーを微調整できます。</span><span class="sxs-lookup"><span data-stu-id="053e9-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="053e9-113">**保護するユーザーを追加する:** この例では、少なくとも CEO のメール アドレスを追加します。</span><span class="sxs-lookup"><span data-stu-id="053e9-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="053e9-114">**保護するドメインを追加する**: CEO のオフィスを含む組織のドメインを追加します。</span><span class="sxs-lookup"><span data-stu-id="053e9-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="053e9-115">**アクションの選択**: **偽装されたユーザーによってメールが送信された場合** は、[**メッセージを別のメール アドレスにリダイレクトする**] を選び、セキュリティ管理者のメール アドレス ( *securityadmin@contoso.com* など) を入力します。</span><span class="sxs-lookup"><span data-stu-id="053e9-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="053e9-116">**偽装されたドメイン アカウントによってメールを送信された場合** は、[**メッセージを検疫**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="053e9-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="053e9-117">**メールボックス インテリジェンス**: 規定では、新しいフィッシング対策ポリシーの作成時にはこのオプションが選択されています。</span><span class="sxs-lookup"><span data-stu-id="053e9-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="053e9-118">最適な結果が得られるように、この設定は **[オン]** のままにしておいてください。</span><span class="sxs-lookup"><span data-stu-id="053e9-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="053e9-119">**信頼できる差出人とドメインを追加する:** この例では、上書きを定義しないでください。</span><span class="sxs-lookup"><span data-stu-id="053e9-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="053e9-120">設定を確認したら、必要に応じて [**このポリシーを作成する**] または [**保存する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="053e9-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="053e9-121">詳細については、「[Microsoft 365 のフィッシング詐欺対策ポリシー](https://go.microsoft.com/fwlink/?linkid=2092235)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="053e9-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
