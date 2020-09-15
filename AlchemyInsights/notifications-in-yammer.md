---
title: Yammer の通知
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: c1fbeea7bf4269e90e52cf5c129e904c99714926
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662798"
---
# <a name="notifications-in-yammer"></a>Yammer の通知

関連する会話で新しいアクティビティがあることをユーザーに通知するため、メールまたはプッシュ通知 (Yammer をモバイル デバイスで使用している場合) により、[Yammer から通知が送信されます](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)。 既定では、ネットワーク内のさまざまな種類のアクティビティに関する通知が Yammer により送信されます。 ユーザーは、Yammer Web サイトからメール設定を更新できます。また、モバイル アプリからプッシュ通知を設定できます。 

Yammer に、[Outlook の対話型メール](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420)のサポートが追加されました。 一部のメール (メッセージのコピー) は、Outlook on the web 内では対話型になります。 今後の更新プログラムで、他のバージョンの Outlook でもこの機能が提供される予定です。

**Yammer の通知の種類**

- メール (グループからの更新、自分が他のユーザーからグループに招待された場合、受信トレイにメッセージを受信した場合など)。
- プッシュ通知 (自分がメンションされた場合、受信トレイにメッセージを受信した場合などにモバイル デバイスに送信されます)。
- デスクトップ ポップアップ (Yammer デスクトップ アプリがインストールされている場合、"トースト" 通知と呼ばれる通知がユーザーに対して表示されます)。
- ベル通知 (Yammer Web サイト内に、さまざまなイベントの通知が表示されます。 これらの通知には、関連付けられたメールやプッシュ通知が存在しない場合があります)。

詳細については、[通知に関する詳細情報](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)を参照してください。

**通知の管理**

ユーザーは、自分の通知を管理する必要があります。 詳細については、「[Yammer メールおよびモバイル通知を有効または無効にする方法](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)」を参照してください。 

すべての通知の無効化や通知の管理を、管理者がユーザーに代わって行うことはできません。 管理者は、[メールに含まれるロゴ、およびメールで投稿されたメッセージをユーザーが確認する必要があるかどうかを制御する](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer)ことができます。

**組織内の多数のユーザーに送信されるメール通知**

Yammer によって送信された 1 通のメール通知を、予想よりもはるかに多くのユーザーが受信する場合があります。 これは、配布リストや他の種類の個人のメール アドレス以外のものが Yammer に追加されている場合に発生します。 Yammer では、あるメール アドレスが 1 人のユーザーに属しているか、1 通のメールが多くの受信者に配信されるようなメール アドレスであるのかを、常に識別できる訳ではありません。 この問題が発生する場合は、Yammer で[そのメール アドレスを持つ無効なユーザーを一時停止 (非アクティブ化) する](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)ための操作を行う必要があります。 

この問題が発生する可能性を減らすには、次の操作を行います。

1. Yammer に [Office 365 ID を適用](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)します。
2. 外部の送信者がお客様の組織にメールを送信できないようにブロックするか、送信者を承認済みのリストに制限します。

この問題が発生する場合:

1. メールの受信者を特定します。これは Yammer のユーザーと一致している必要があります。 たとえば、all-in-sales@fabrikam.com は営業担当者全員を対象とした DL です。 この DL は、ユーザーが受信した Yammer メールから識別できます。
2. [ネットワーク管理者の非アクティブ化 (一時停止) 機能](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)を使用して、all-in-sales@fabrikam.com というメール アドレスを持つユーザーを一時停止します。 一時停止は取り消すことができるので、削除よりも安全です。 ユーザーの削除は、90 日後に自動的に実行されます。
3. 必要に応じて、[[User Export]\(ユーザー情報をエクスポートする\)](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) を確認し、ユーザーのメール アドレスではない、一時停止する必要がある他のものを特定します。
