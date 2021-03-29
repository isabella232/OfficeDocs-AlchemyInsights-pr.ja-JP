---
title: バックスキャター攻撃からの保護
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038269"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="054bb-102">バックスキャター攻撃からの保護</span><span class="sxs-lookup"><span data-stu-id="054bb-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="054bb-103">バックスキャターは、送信されなかったメッセージに対して受信する、配信不能レポート (NDR またはバウンス メッセージとも呼ばれるもの) です。</span><span class="sxs-lookup"><span data-stu-id="054bb-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="054bb-104">スパム送信者は、メッセージの **送信者** アドレスを偽装 (なりすまし) し、メッセージへの信頼性を高めるために、実在するメール アドレスを使用することがよくあります。</span><span class="sxs-lookup"><span data-stu-id="054bb-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="054bb-105">したがって、スパム送信者が、存在しない受信者にメッセージを送信すると、宛先のメール サーバーは、NDR の配信不能メッセージを偽装された **送信者** アドレスに返すようにだまされます。</span><span class="sxs-lookup"><span data-stu-id="054bb-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="054bb-106">追加情報については、「[EOP のバックスキャター](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="054bb-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="054bb-107">**バックスキャター保護の有効化**</span><span class="sxs-lookup"><span data-stu-id="054bb-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="054bb-108">バックスキャター保護を有効にするには、次のパスに従います。</span><span class="sxs-lookup"><span data-stu-id="054bb-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="054bb-109">**protection.office.com > 脅威の管理 > ポリシー > スパム対策 > スパム フィルター ポリシーと編集ポリシーの選択 > スパム プロパティ > スパムとしてチェック > NDR バックスキャター > [オン] に設定する**</span><span class="sxs-lookup"><span data-stu-id="054bb-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="054bb-110">アカウントが侵害されたと思われる場合は、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="054bb-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="054bb-111">侵害された電子メール アカウントへの対応</span><span class="sxs-lookup"><span data-stu-id="054bb-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="054bb-112">Office 365 の制限されたユーザー ポータルから、ブロックされたユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="054bb-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



