---
title: TLS 1.0 および TLS 1.1 の無効化のため、Office 365 でメールを送受信できない
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
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751149"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="56292-102">TLS 1.0 および TLS 1.1 の無効化のため、Office 365 でメールを送受信できない</span><span class="sxs-lookup"><span data-stu-id="56292-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="56292-103">メッセージ センターの投稿 MC229914 で確認された、TLS 1.0 と TLS 1.1 の廃止が Exchange Online のメール フロー エンドポイントへの適用を開始しました。</span><span class="sxs-lookup"><span data-stu-id="56292-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="56292-104">まもなく、Office 365 は外部ソースからの TLS 1.0 と TLS 1.1 メール接続を受け入れなくなります。</span><span class="sxs-lookup"><span data-stu-id="56292-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="56292-105">また、Exchange Online は TLS 1.0 または 1.1 を使用してメールを送信することはなくなります。</span><span class="sxs-lookup"><span data-stu-id="56292-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="56292-106">TLS 1.0 または 1.1 の無効化による問題が発生している場合は、次のいずれかのエラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="56292-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="56292-107">送信者が NDR バウンス バックを受信している - '421 4.4.2 SocketError により接続がドロップされました'</span><span class="sxs-lookup"><span data-stu-id="56292-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="56292-108">Officer 365 - '421 4.4.2 SocketError により接続がドロップされたオンプレミス サーバーのキュー ビューアーのエラー'</span><span class="sxs-lookup"><span data-stu-id="56292-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="56292-109">Office 365 にメールを送信するサーバーのコネクタ [プロトコル ログ](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging)の送信エラー: TLS ネゴシエーションが SocketError エラーによって失敗しました</span><span class="sxs-lookup"><span data-stu-id="56292-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="56292-110">コネクタ プロトコル ログの送受信のエラー - '451 5.7.3 最初に STARTTLS コマンドを発行する必要があります'</span><span class="sxs-lookup"><span data-stu-id="56292-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="56292-111">上記のエラーが発生した場合は、メールの送受信サーバーで TLS 1.2 が有効になっているかどうかを、次のレジストリ キーから確認します。</span><span class="sxs-lookup"><span data-stu-id="56292-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="56292-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="56292-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="56292-113">TLS 1.2 を有効にするために上記のレジストリ キーを変更した場合は、サーバーを再起動して変更を有効にします。</span><span class="sxs-lookup"><span data-stu-id="56292-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="56292-114">また、最新の Windows と Exchange の更新プログラムがインストールされていることも確認します。</span><span class="sxs-lookup"><span data-stu-id="56292-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="56292-115">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56292-115">For more information, see:</span></span>

- [<span data-ttu-id="56292-116">Exchange Server TLS ガイダンス、パート 1: TLS 1.2 の準備 - Microsoft 技術コミュニティ</span><span class="sxs-lookup"><span data-stu-id="56292-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="56292-117">Exchange サーバー TLS ガイダンス パート 2: TLS 1.2 を有効にして、それを使用していないクライアントを特定する - Microsoft 技術コミュニティ</span><span class="sxs-lookup"><span data-stu-id="56292-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="56292-118">TLS バージョンが Exchange Online で合意できない場合のメール シナリオを理解する - Microsoft 技術コミュニティ</span><span class="sxs-lookup"><span data-stu-id="56292-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
