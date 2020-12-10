---
title: Microsoft Edge での Microsoft Defender Application Guard のサポート
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584218"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge での Microsoft Defender Application Guard のサポート

Windows 10 および Microsoft Edge 用に設計された Application Guard は、ハードウェア分離アプローチを使用して、ユーザーがホスト オペレーティング システムから分離された Hyper-V 対応コンテナー内から信頼できないサイトをナビゲートできるようにします。

エンタープライズ管理者は、信頼済みサイト、クラウド リソース、内部ネットワークの一覧を定義します。 ユーザーが一覧にないサイトにアクセスすると、そのサイトが Microsoft Edge でコンテナーに表示されます。 これは、サイトが悪意のあるものであることが判明した場合、ホスト PC は保護され、攻撃者は会社のデータにアクセスできなくなることを意味します。

コンテナーへの拡張機能のインストールは、Microsoft Edge バージョン 81 以降でサポートされており、ポリシーを通して制御できます。 ポリシーで使用される ExtensionInstallForcelist は、Application Guard が使用するネットワークの分離ポリシーでニュートラル リソースとして追加する必要があります。

詳細については、「[Microsoft Edge での Microsoft Defender Application Guard のサポート](https://go.microsoft.com/fwlink/?linkid=2134229)」を参照してください。
