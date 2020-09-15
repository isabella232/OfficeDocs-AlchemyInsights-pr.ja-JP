---
title: Teams 管理センター
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
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670369"
---
# <a name="teams-admin-center"></a>Teams 管理センター

[Teams 管理センター](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)を使用して、Teams を管理する方法について説明します。

Teams 管理センターにアクセスできない場合は、以下の項目を確認してください。

- すべての境界デバイス (ファイアウォールなど) またはローカル コンピューター上のファイアウォール規則で適切な [Office 365 の IP アドレスと URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) を許可していることを確認します。
- Teams 管理ポータルへのアクセスに使用しているログイン ユーザー名が、[Microsoft 365 管理ポータル](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)に登録されているユーザー名と一致していることを確認します。

Teams 管理センターでユーザーが表示されない場合は、以下の項目を確認してください。

- 24 時間以内にユーザーの作成、またはライセンスの割り当てを行ったかどうか。 サポート チケットをオープンする前に 24 時間以上経過したことをご確認ください。
- 適切なライセンスが割り当てられていることを確認したか。
- オンプレミスの Active Directory がある場合は、[msRTCSIP-PrimaryUserAddress の値またはローカル Active Directory の ProxyAddresses フィールドの SIP アドレスが一意であり、形式が一致していることを確認します](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) (sip: [Microsoft 365 管理センター](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)のユーザーの **Username**)。
- Skype for Business Server の展開を維持し、ユーザーをオンプレミスおよびオンラインに置く場合は、Skype for Business Server コントロール パネルの **「Teams および Skype for Business Online とのハイブリッドのセットアップ」** に従ってください。ユーザーをオンラインに移動します。
