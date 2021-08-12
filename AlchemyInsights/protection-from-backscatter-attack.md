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
ms.openlocfilehash: 8c6b1cfe79d322702279877ff351397a366fa246710c04e25181a675ad2fdeab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911235"
---
# <a name="protection-from-backscatter-attack"></a>バックスキャター攻撃からの保護

バックスキャターは、送信されなかったメッセージに対して受信する、配信不能レポート (NDR またはバウンス メッセージとも呼ばれるもの) です。 スパム送信者は、メッセージの **送信者** アドレスを偽装 (なりすまし) し、メッセージへの信頼性を高めるために、実在するメール アドレスを使用することがよくあります。 したがって、スパム送信者が、存在しない受信者にメッセージを送信すると、宛先のメール サーバーは、NDR の配信不能メッセージを偽装された **送信者** アドレスに返すようにだまされます。

追加情報については、「[EOP のバックスキャター](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)」を参照してください。

**バックスキャター保護の有効化**

バックスキャター保護を有効にするには、次のパスに従います。

**protection.office.com > 脅威の管理 > ポリシー > スパム対策 > スパム フィルター ポリシーと編集ポリシーの選択 > スパム プロパティ > スパムとしてチェック > NDR バックスキャター > [オン] に設定する**

アカウントが侵害されたと思われる場合は、次を参照してください。

- [侵害された電子メール アカウントへの対応](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Office 365 の制限されたユーザー ポータルから、ブロックされたユーザーを削除する](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



