---
title: 2681 Microsoft 365 の攻撃シミュレータ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545731"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="5b694-102">Microsoft 365 の攻撃シミュレータ</span><span class="sxs-lookup"><span data-stu-id="5b694-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="5b694-103">攻撃シミュレータが見つかりませんか ?</span><span class="sxs-lookup"><span data-stu-id="5b694-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="5b694-104">攻撃シミュレータには、**Microsoft Defender for Office 365 プラン 2** または **Office 365 Enterprise E5** が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b694-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="5b694-105">攻撃シミュレータは、Microsoft Defender for Office 365 プラン 1、Office 365 Enterprise E3、または Microsoft 365 Apps for business サブスクリプションには含まれて **いません**。</span><span class="sxs-lookup"><span data-stu-id="5b694-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="5b694-106">シミュレートされた攻撃を開始するために使用するアカウントには、グローバル管理者またはセキュリティ管理者のアクセス許可および多要素認証 (MFA) が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b694-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="5b694-107">攻撃シミュレータの要件の詳細情報については、[このトピック](/microsoft-365/security/office-365-security/attack-simulator)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b694-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="5b694-108">**ブルート フォース パスワード** 攻撃シミュレーションに関する重要な注意事項:</span><span class="sxs-lookup"><span data-stu-id="5b694-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="5b694-109">ターゲット アカウントで MFA が有効になっており、パスワードが正しく推測された場合、アカウントは危険にさらされているものとして表示されません (2 番目の認証要素は不完全です)。</span><span class="sxs-lookup"><span data-stu-id="5b694-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="5b694-110">パスワード ファイルは 10 MB を超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="5b694-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="5b694-111">1 行に 1 つのパスワードを使用し、リストの最後のパスワードの後に空白行 (キャリッジ リターン) を含めます。</span><span class="sxs-lookup"><span data-stu-id="5b694-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="5b694-112">**スピア フィッシング** 攻撃のシミュレーションに関する重要な注意事項:</span><span class="sxs-lookup"><span data-stu-id="5b694-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="5b694-113">仕様上、**フィッシング ログイン サーバーの URL** にカスタム値を指定することはできません。</span><span class="sxs-lookup"><span data-stu-id="5b694-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="5b694-114">受信者が[レポート メッセージ アドインを有効にする](/microsoft-365/security/office-365-security/enable-the-report-message-add-in)を使用してメッセージをフィッシングとして報告する場合、メッセージのアラートを受信しない場合があります (シミュレートされた攻撃であるため)。</span><span class="sxs-lookup"><span data-stu-id="5b694-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="5b694-115">レポート: シミュレートされた攻撃が完了したら、[**攻撃の詳細**] をクリックしてレポートを確認できます。</span><span class="sxs-lookup"><span data-stu-id="5b694-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="5b694-116">攻撃シミュレータの詳細な手順および新機能については、「[Microsoft 365 の攻撃シミュレータ](/microsoft-365/security/office-365-security/attack-simulator)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b694-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
