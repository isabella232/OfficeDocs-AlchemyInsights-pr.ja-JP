---
title: アプリの互換性テストを行う
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50696436"
---
# <a name="do-app-compatibility-testing"></a>アプリの互換性テストを行う

Microsoft Edge のアプリケーションの互換性は非常に高いです。 実際に、Microsoft が次の互換性の保証を提供するほど、非常に高いレベルです。
- Microsoft Edge 45 以前のバージョンで動作する場合、Microsoft Edge 77 以降のバージョンでも動作します。
- Internet Explorer で動作する場合は、Internet Explorer モードの Microsoft Edge でも動作します。
- Google Chrome で動作する場合、Microsoft Edge で動作します。

この保証を満たしないアプリケーションがある場合、Microsoft アプリ Assure[ 修正することを確約いたします](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)。

こうした確約はあるものの、多くの組織は、コンプライアンスまたはリスク管理の理由で、一部のアプリケーションを検証する必要があります。 この手順は非常に簡単になるものと予想していましたが、アプリのテストにおいては組織化され、厳密であることが重要になります。

アプリの互換性テストを行うには 2 つの方法があります。

- **ラボ テスト**: アプリケーションは、特定の構成を使用して、厳密にコントロールされた環境でテストされます。
- **パイロット テスト**: アプリケーションは、限定された数のユーザーが、自分のデバイスを使用し、日常の作業環境の中でテストされます。 

各アプリに最も適した方法を選び、組織全体にリリースする前にテストを行います。

アプリと互換性を確認したら、Microsoft Edge をパイロット グループに展開する準備が整ったことになります。
