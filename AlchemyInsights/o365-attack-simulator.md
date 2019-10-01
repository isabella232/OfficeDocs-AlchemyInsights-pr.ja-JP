---
title: Office 365 の2681アタックシミュレータ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2019
ms.locfileid: "37313941"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="517b9-102">Office 365 の攻撃シミュレータ</span><span class="sxs-lookup"><span data-stu-id="517b9-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="517b9-103">アタックシミュレータはありませんか?</span><span class="sxs-lookup"><span data-stu-id="517b9-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="517b9-104">アタックシミュレータには、 **office 365 Advanced Threat Protection プラン 2 (ATP Plan 2)** または**Office 365 Enterprise E5**が必要です。</span><span class="sxs-lookup"><span data-stu-id="517b9-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="517b9-105">アタックシミュレータは、Office 365 Advanced Threat Protection プラン 1 (ATP プラン 1)、Office 365 Enterprise E3、または任意の Office 365 Business サブスクリプションに含まれて**いません**。</span><span class="sxs-lookup"><span data-stu-id="517b9-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="517b9-106">シミュレートされた攻撃を開始するために使用するアカウントには、グローバル管理者またはセキュリティ管理者のアクセス許可と多要素認証 (MFA) が必要です。</span><span class="sxs-lookup"><span data-stu-id="517b9-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="517b9-107">アタックシミュレータの要件の詳細については、[このトピック](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="517b9-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="517b9-108">**ブルートフォースパスワード**攻撃のシミュレーションに関して知っておくべき重要な点は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="517b9-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="517b9-109">ターゲットアカウントの MFA が有効になっており、パスワードが正しく推測されている場合、そのアカウントは侵害されたとして表示されません (2 番目の認証要素は不完全になります)。</span><span class="sxs-lookup"><span data-stu-id="517b9-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="517b9-110">パスワードファイルは、10 MB を超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="517b9-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="517b9-111">行ごとに1つのパスワードを使用し、リスト内の最後のパスワードの後に空白行 (復帰) を含めます。</span><span class="sxs-lookup"><span data-stu-id="517b9-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="517b9-112">**スピアーフィッシング**接続のシミュレーションに関して知っておくべき重要な点は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="517b9-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="517b9-113">設計上、**フィッシングのログインサーバーの URL**にカスタム値を指定することはできません。</span><span class="sxs-lookup"><span data-stu-id="517b9-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="517b9-114">受信者が [[レポートメッセージを有効](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)にする] アドインを使用してメッセージをフィッシングとして報告する場合、メッセージの通知を受信しないことがあります (これはシミュレートされた攻撃です)。</span><span class="sxs-lookup"><span data-stu-id="517b9-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="517b9-115">レポート: シミュレートされた攻撃が完了したら、[**アタックの詳細**] をクリックしてレポートを表示できます。</span><span class="sxs-lookup"><span data-stu-id="517b9-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="517b9-116">アタックシミュレータの詳細な手順と新機能については、「 [Office 365 のアタックシミュレータ](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="517b9-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
