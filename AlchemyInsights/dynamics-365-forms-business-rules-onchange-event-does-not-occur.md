---
title: Dynamics 365 のフォーム ビジネス ルール - フォームに対して、ビジネス ルールが生成されない
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947304"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>プログラムでフィールドが変更されている場合、OnChange イベントは発生しません。

*OnChange* イベントは、*attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) メソッドを使用するプログラムでフィールドが変更されている場合には発生しません。 値を設定してから *OnChange* イベントのイベント ハンドラーを実行するには、コードで *formContext.data.entity attribute.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) メソッドを使用する必要があります。

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
