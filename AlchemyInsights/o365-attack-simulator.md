---
title: 2681 Microsoft 365 の攻撃シミュレータ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713471"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="115c2-102">Microsoft 365 の攻撃シミュレータ</span><span class="sxs-lookup"><span data-stu-id="115c2-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="115c2-103">攻撃シミュレータが見つかりませんか ?</span><span class="sxs-lookup"><span data-stu-id="115c2-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="115c2-104">攻撃シミュレータには、**Office 365 Advanced Threat Protection プラン 2 (ATP プラン 2)** または **Office 365 Enterprise E5** が必要です。</span><span class="sxs-lookup"><span data-stu-id="115c2-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="115c2-105">攻撃シミュレータは、Office 365 Advanced Threat Protection プラン 1 (ATP プラン 1)、Office 365 Enterprise E3、または 一般法人向け Microsoft 365 アプリ サブスクリプションには含まれて**いません**。</span><span class="sxs-lookup"><span data-stu-id="115c2-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="115c2-106">シミュレートされた攻撃を開始するために使用するアカウントには、グローバル管理者またはセキュリティ管理者のアクセス許可および多要素認証 (MFA) が必要です。</span><span class="sxs-lookup"><span data-stu-id="115c2-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="115c2-107">攻撃シミュレータの要件の詳細情報については、[このトピック](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="115c2-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="115c2-108">**ブルート フォース パスワード**攻撃シミュレーションに関する重要な注意事項:</span><span class="sxs-lookup"><span data-stu-id="115c2-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="115c2-109">ターゲット アカウントで MFA が有効になっており、パスワードが正しく推測された場合、アカウントは危険にさらされているものとして表示されません (2 番目の認証要素は不完全です)。</span><span class="sxs-lookup"><span data-stu-id="115c2-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="115c2-110">パスワード ファイルは 10 MB を超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="115c2-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="115c2-111">1 行に 1 つのパスワードを使用し、リストの最後のパスワードの後に空白行 (キャリッジ リターン) を含めます。</span><span class="sxs-lookup"><span data-stu-id="115c2-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="115c2-112">**スピア フィッシング**攻撃のシミュレーションに関する重要な注意事項:</span><span class="sxs-lookup"><span data-stu-id="115c2-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="115c2-113">仕様上、**フィッシング ログイン サーバーの URL** にカスタム値を指定することはできません。</span><span class="sxs-lookup"><span data-stu-id="115c2-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="115c2-114">受信者が[レポート メッセージ アドインを有効にする](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)を使用してメッセージをフィッシングとして報告する場合、メッセージのアラートを受信しない場合があります (シミュレートされた攻撃であるため)。</span><span class="sxs-lookup"><span data-stu-id="115c2-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="115c2-115">レポート: シミュレートされた攻撃が完了したら、[**攻撃の詳細**] をクリックしてレポートを確認できます。</span><span class="sxs-lookup"><span data-stu-id="115c2-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="115c2-116">攻撃シミュレータの詳細な手順および新機能については、「[Microsoft 365 の攻撃シミュレータ](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="115c2-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
