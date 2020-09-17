---
title: セキュリティ センターにサブスクリプションが見つかりませんというメッセージ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772609"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>セキュリティ センターにサブスクリプションが見つかりませんというメッセージ

Microsoft Defender セキュリティ センターにアクセスしているときに「サブスクリプションが見つかりません」というメッセージが表示される場合は、ポータルへのユーザーのログインに使用される Azure Active Directory (AAD) に Microsoft Defender ATP ライセンスがないことを意味します。  

Windows E5 ライセンスと Office E5 ライセンスは、別のライセンスです。

ライセンスを購入したが、この AAD インスタンスにプロビジョニングされていない場合は、サポート案件をオープンします。 次のいずれかがあります: <br/>
-   可能性のあるライセンスのプロビジョニングの問題。<br/>
-   ユーザーが、サービスへの認証に使用されたものとは異なる Microsoft AAD に誤ってライセンスをプロビジョニングしました。