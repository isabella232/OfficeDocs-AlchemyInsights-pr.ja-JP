---
title: ポータルで重複しているデバイス レコード
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "43791316"
---
# <a name="duplicate-device-record-in-the-portal"></a>ポータルで重複しているデバイス レコード

ポータルで、1 つのデバイスに対して 2 つのレコードが表示されることがあります。これは、そのデバイスが共同管理の状態を Configuration Manager サイトに正しく報告していない場合に発生します。 デバイスの共同管理の状態を調べるには、Configuration Manager コンソールでデバイスの **[共同管理]** 列を確認します。 この列が表示されていない場合は、任意の列見出しを右クリックして、リストから目的の列を選択することで追加できます。

[共同管理] の値は、**[はい]** になっている必要があります。 この値が **[いいえ]** の場合は、クライアント デバイスで Configuration Manager クライアント アプレットを起動して、[全般] タブで **[Co-management]** プロパティを確認します。

- この値が **[Enabled]** の場合は、クライアントと管理ポイントとの通信に問題があることを示しています。 デバイスの **CcmMessaging.log** を確認して、可能性のある接続の問題を調査してください。

- この値が **[Disabled]** のときに、デバイスが Intune で登録されている場合は、デバイスの **CoManagementHandler.log** を調べて、デバイスが共同管理ポリシーを受け取っていることを確認してください。
