---
title: Intune デバイス インベントリ
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667883"
---
# <a name="intune-device-inventory"></a>Intune デバイス インベントリ

デバイス ブレードは、デバイスごとに Intune で管理されているデバイスに対する管理者の分析情報を提供します。 表示される情報には、ハードウェア、検出されたアプリケーション、デバイスのコンプライアンス状態、デバイスの構成状態が含まれます。

ハードウェアと検出されたアプリケーションのインベントリデータは、7日間のサイクルで収集されます。 報告されるハードウェアのアプリケーションと特定の要素は、デバイスのオペレーティングシステムとデバイスが個人所有か企業所有かによって異なります。

詳細については、「[Intuneでデバイスの詳細を確認する](https://docs.microsoft.com/intune/device-inventory)」を参照してください。

**FAQ**

Q: Intune に登録された Windows デバイスに存在するアプリケーションの完全なインベントリリストを受け取っていません。 どうしてでしょうか?

A: 現時点では、企業のデバイスとして識別される Windows 10 PC 用の最新アプリのみがリスト表示されます。 Intune は、これらのデバイスにインストールされているWin32 アプリに関する情報を収集しません。

Q: どのデバイスからも電話番号が収集されないのはなぜですか?

A: Intune で企業デバイスとして分類された電話は、モバイルデバイス インベントリレポートを実行したときなどは、完全な電話番号として識別されません。 持ち込まれたデバイスの電話番号は、部分的にアスタリスク (****) で隠され、最後の4桁のみが表示されます。