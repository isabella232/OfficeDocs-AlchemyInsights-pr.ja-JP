---
title: Microsoft Intune セキュリティ ベースラインを使用して Windows 10 デバイスを構成する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104349"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Microsoft Intune セキュリティ ベースラインを使用して Windows 10 デバイスを構成する

Intune セキュリティ ベースラインは、ユーザーとデバイスを保護するのに役立ちます。 セキュリティ ベースラインは事前構成済みの Windows 設定のグループで、関連するセキュリティ チームが推奨する一連の設定と既定値を適用するために使用されます。 Intune でセキュリティ ベースラインのプロファイルを作成することで、複数のデバイス構成プロファイルで構成されたテンプレートを作成します。

ユーザーやデバイスのグループに対してセキュリティ ベースラインを展開すると、Windows 10 以降を実行するデバイスに設定が適用されます。 たとえば、MDM セキュリティ ベースラインを使用すると、自動的に (1) リムーバブル ドライブに対する BitLocker の有効化、(2) デバイスのロックを解除するためのパスワードの要求、(3) プレーンテキスト認証の無効化が実行されます。 既定値がご利用の環境でうまく機能しない場合は、ベースラインをカスタマイズして必要な設定を適用してください。

セキュリティ ベースラインは、セキュリティで保護されたエンド ツー エンドのワークフローを Microsoft 365 で確立するのにも役立ちます。 これには次のような利点があります。

- セキュリティ ベースラインには、セキュリティに影響を与える設定のベスト プラクティスとおすすめが含まれています。 Intune はグループ ポリシーのベースラインを作成する Windows セキュリティ チームと連携を図っているため、このようなおすすめは正確なガイダンスと豊富な経験に基づいています。
- Intune を使用したことがなく、どこから手を付けたらよいか分からない場合、セキュリティ ベースラインはセキュリティで保護されたプロファイルをすばやく作成して展開するのに役立ちます。
- セキュリティ ベースラインは Intune に組み込まれており、管理に使用できる最先端の機能が含まれています。そのため、現在グループ ポリシーを使用している場合は、セキュリティ ベースラインを使用すると、管理目的で Intune に移行する作業がはるかに簡単になります。

詳細については、「[Windows セキュリティ ベースライン](https://go.microsoft.com/fwlink/?linkid=2141503)」および「[モバイル デバイス管理](https://go.microsoft.com/fwlink/?linkid=2141701)」を参照してください。