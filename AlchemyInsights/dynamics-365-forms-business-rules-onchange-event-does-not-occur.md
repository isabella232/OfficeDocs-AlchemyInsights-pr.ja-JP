---
title: Dynamics 365 のフォーム ビジネス ルール - フォームに対して、ビジネス ルールが生成されない
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35760734"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>プログラムでフィールドが変更されている場合、OnChange イベントは発生しません。

*OnChange* イベントは、*属性*[setValue](https://docs.microsoft.com/ja-JP/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) メソッドを使用するプログラムでフィールドが変更されている場合には発生しません。 値を設定してから *OnChange* イベントのイベント ハンドラーを実行するには、コードで*formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/ja-JP/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)メソッドを使用する必要があります。

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
