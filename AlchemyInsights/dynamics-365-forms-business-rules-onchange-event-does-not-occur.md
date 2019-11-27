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
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769344"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="4e0e5-102">プログラムでフィールドが変更されている場合、OnChange イベントは発生しません。</span><span class="sxs-lookup"><span data-stu-id="4e0e5-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="4e0e5-103">*OnChange* イベントは、*attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) メソッドを使用するプログラムでフィールドが変更されている場合には発生しません。</span><span class="sxs-lookup"><span data-stu-id="4e0e5-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="4e0e5-104">値を設定してから *OnChange* イベントのイベント ハンドラーを実行するには、コードで *formContext.data.entity attribute.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) メソッドを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e0e5-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
