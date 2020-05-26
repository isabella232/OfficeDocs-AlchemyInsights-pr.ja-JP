---
title: Teams 管理センター
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354093"
---
# <a name="teams-admin-center"></a><span data-ttu-id="886ec-102">Teams 管理センター</span><span class="sxs-lookup"><span data-stu-id="886ec-102">Teams Admin Center</span></span>

<span data-ttu-id="886ec-103">[Teams 管理センター](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)を使用して、Teams を管理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="886ec-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="886ec-104">Teams 管理センターにアクセスできない場合は、以下の項目を確認してください。</span><span class="sxs-lookup"><span data-stu-id="886ec-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="886ec-105">すべての境界デバイス (ファイアウォールなど) またはローカル コンピューター上のファイアウォール規則で適切な [Office 365 の IP アドレスと URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) を許可していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="886ec-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="886ec-106">Teams 管理ポータルへのアクセスに使用しているログイン ユーザー名が、[Microsoft 365 管理ポータル](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)に登録されているユーザー名と一致していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="886ec-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="886ec-107">Teams 管理センターでユーザーが表示されない場合は、以下の項目を確認してください。</span><span class="sxs-lookup"><span data-stu-id="886ec-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="886ec-108">24 時間以内にユーザーの作成、またはライセンスの割り当てを行ったかどうか。</span><span class="sxs-lookup"><span data-stu-id="886ec-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="886ec-109">サポート チケットをオープンする前に 24 時間以上経過したことをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="886ec-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="886ec-110">適切なライセンスが割り当てられていることを確認したか。</span><span class="sxs-lookup"><span data-stu-id="886ec-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="886ec-111">オンプレミスの Active Directory がある場合は、[msRTCSIP-PrimaryUserAddress の値またはローカル Active Directory の ProxyAddresses フィールドの SIP アドレスが一意であり、形式が一致していることを確認します](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) (sip: [Microsoft 365 管理センター](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)のユーザーの **Username**)。</span><span class="sxs-lookup"><span data-stu-id="886ec-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="886ec-112">Skype for Business Server の展開を維持し、ユーザーをオンプレミスおよびオンラインに置く場合は、Skype for Business Server コントロール パネルの **「Teams および Skype for Business Online とのハイブリッドのセットアップ」** に従ってください。ユーザーをオンラインに移動します。</span><span class="sxs-lookup"><span data-stu-id="886ec-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
