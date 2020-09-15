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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711496"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="b6d60-102">プログラムでフィールドが変更されている場合、OnChange イベントは発生しません。</span><span class="sxs-lookup"><span data-stu-id="b6d60-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="b6d60-103">*OnChange* イベントは、*attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) メソッドを使用するプログラムでフィールドが変更されている場合には発生しません。</span><span class="sxs-lookup"><span data-stu-id="b6d60-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="b6d60-104">値を設定してから *OnChange* イベントのイベント ハンドラーを実行するには、コードで *formContext.data.entity attribute.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) メソッドを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6d60-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
