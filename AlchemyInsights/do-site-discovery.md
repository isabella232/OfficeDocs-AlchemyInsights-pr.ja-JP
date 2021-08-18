---
title: サイト探索を行う
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
- "9143"
- "9005291"
ms.openlocfilehash: 5ae99192c769dd5d5acae1c6e8f9b021e824b465
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322172"
---
# <a name="do-site-discovery"></a>サイト探索を行う

レガシ Web アプリケーションをまだ使用しており、Internet Explorer モードの使用を計画している場合 (ほとんどのお客様が該当)、追加のサイト探索の実行が必要になる可能性があります。

**Microsoft Edge の以前のバージョンが既に展開されています**

Microsoft Edge のレガシ バージョンで使用するように、エンタープライズ サイト一覧が既に構成されている場合、サイト探索はほぼ完了しています。 ニュートラル サイトの追加が必要になる場合があります。

ニュートラルサイトは、通常、シングル サインオン (SSO) を提供するサイトです。 Microsoft Edge からニュートラル サイトに移動する場合は、Microsoft Edge で認証する必要があります。 Internet Explorer モードでニュートラル サイトに移動する場合は、Internet Explorer モードで認証する必要があります。

使用する SSO またはその他のニュートラル サイトを特定し、エンタープライズ サイト一覧に追加します。

**既定のブラウザーが Internet Explorer の場合**

現在、Internet Explorer のみを使用している場合は、どのサイトが最新の Web 標準にアップグレードされ、どのサイトでまだ Internet Explorer が必要であるかを把握していない可能性があります。 これらのサイトを検索して、エンタープライズ サイト一覧に追加する必要があります。 これにより、必要なサイトでのみ Internet Explorer モードを使用できます。

**注**: [Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) を使用して、Internet Explorer モードを必要とする可能性があるサイトを検出します。 Windows 10、Windows 8.1、Windows 7 で、Windows Internet Explorer 8 から Internet Explorer 11 までを実行しているコンピューターでデータを収集できます。

**データを分析する**

サイト データを収集した後、次の 4 つの手順を実行してデータを分析することをお勧めします。
1. データをドメインごと、次に URL ごとに並べ替えます。
2. Internet Explorer モード用に構成するアプリの境界を定義します。 アプリを定義するすべてのサイトと Web コントロールを含める必要があります。ただし、余分なサイトやコントロールを含めないようにします。 サイトによって、*https://contoso.com/app1* ように単純なものもあれば、複数のサイトやページを定義する必要があるものもあります。
3. アプリをテストして、ネイティブに機能していないことを確認します。多くのサイトでは、最新のブラウザーが検出されると最新のコンテンツが提供され、Internet Explorer が検出された場合にのみレガシ コンテンツが提供されます。
4. アプリがテストで失敗した場合は、エンタープライズ サイト一覧にアプリを追加します。

**注**: ベスト プラクティスとして、アプリを構成するすべてのサイトをグループ化することをお勧めします。 これにより、アプリをアップグレードするときに、サイト全体を Internet Explorer モードから削除し、そのアプリに最新のブラウザーを使用し始めるのが簡単になります。

サイト探索とデータの分析が完了すると、チャネル戦略の検索を開始する準備ができています。

