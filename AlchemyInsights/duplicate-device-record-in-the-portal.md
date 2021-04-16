---
title: ポータルで重複しているデバイス レコード
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814521"
---
# <a name="duplicate-device-record-in-the-portal"></a>ポータルで重複しているデバイス レコード

ポータルで、1 つのデバイスに対して 2 つのレコードが表示されることがあります。これは、そのデバイスが共同管理の状態を Configuration Manager サイトに正しく報告していない場合に発生します。 デバイスの共同管理の状態を調べるには、Configuration Manager コンソールでデバイスの **[共同管理]** 列を確認します。 この列が表示されていない場合は、任意の列見出しを右クリックして、リストから目的の列を選択することで追加できます。

[共同管理] の値は、**[はい]** になっている必要があります。 この値が **[いいえ]** の場合は、クライアント デバイスで Configuration Manager クライアント アプレットを起動して、[全般] タブで **[Co-management]** プロパティを確認します。

- この値が **[Enabled]** の場合は、クライアントと管理ポイントとの通信に問題があることを示しています。 デバイスの **CcmMessaging.log** を確認して、可能性のある接続の問題を調査してください。

- この値が **[Disabled]** のときに、デバイスが Intune で登録されている場合は、デバイスの **CoManagementHandler.log** を調べて、デバイスが共同管理ポリシーを受け取っていることを確認してください。
