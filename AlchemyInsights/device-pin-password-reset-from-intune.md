---
title: Intune からデバイスの PIN /パスワードをリセットする
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: 66255fc87a55161158aa4121d68d7ccd04b552ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730992"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="d55fa-102">Intune からデバイスの PIN /パスワードをリセットする</span><span class="sxs-lookup"><span data-stu-id="d55fa-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="d55fa-103">パスコードを削除する、または [パスコードの削除] アクションを使って iOS または Android を実行しているデバイスの Intune で新しいパスコードを作成するようにユーザーに強制させることができます。</span><span class="sxs-lookup"><span data-stu-id="d55fa-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="d55fa-104">このアクションをサポートするのは、特定のオペレーティング システムの種類と仕事用プロファイルの種類のみです。</span><span class="sxs-lookup"><span data-stu-id="d55fa-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="d55fa-105">サポートされているプラットフォーム、およびパスコードのリセット アクションをトリガーする方法については、「[Intune でデバイスのパスコードをリセットまたは削除する](https://docs.microsoft.com/intune/device-passcode-reset)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d55fa-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="d55fa-106">Windows 10 Mobile オペレーティング システムを実行しているデバイスで PIN のリセット アクションを使用して、既存の PIN を新しい値に再設定することができます。</span><span class="sxs-lookup"><span data-stu-id="d55fa-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="d55fa-107">これにより、ユーザーはデバイスのロックを解除し、必要に応じて新しい PIN を設定できます。</span><span class="sxs-lookup"><span data-stu-id="d55fa-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="d55fa-108">詳細については、「[Intune を使用して Windows デバイスのパスコードをリセットする](https://docs.microsoft.com/intune/device-windows-pin-reset)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d55fa-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>