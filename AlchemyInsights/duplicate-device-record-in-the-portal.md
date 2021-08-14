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
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004159"
---
# <a name="duplicate-device-record-in-the-portal"></a>ポータルで重複しているデバイス レコード

ポータルで、1 つのデバイスに対して 2 つのレコードが表示されることがあります。これは、そのデバイスが共同管理の状態を Configuration Manager サイトに正しく報告していない場合に発生します。 デバイスの共同管理の状態を調べるには、Configuration Manager コンソールでデバイスの **[共同管理]** 列を確認します。 この列が表示されていない場合は、任意の列見出しを右クリックして、リストから目的の列を選択することで追加できます。

共同管理の値は、**[はい]** にする必要があります。値が **[いいえ]** の場合は、クライアント デバイスで 構成マネージャー クライアント アプレットを開き、[全般] タブの **[共同管理]** プロパティを確認します。

- この値が **[Enabled]** の場合は、クライアントと管理ポイントとの通信に問題があることを示しています。 デバイスの **CcmMessaging.log** を確認して、可能性のある接続の問題を調査してください。

- この値が **[Disabled]** のときに、デバイスが Intune で登録されている場合は、デバイスの **CoManagementHandler.log** を調べて、デバイスが共同管理ポリシーを受け取っていることを確認してください。
