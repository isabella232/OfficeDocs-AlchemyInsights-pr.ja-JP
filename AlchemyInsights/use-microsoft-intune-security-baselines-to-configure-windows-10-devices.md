---
title: Microsoft Intune セキュリティ ベースラインを使用して Windows 10 デバイスを構成する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696554"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Windows 10 デバイスの構成に Microsoft Intune セキュリティ ベースラインを使用する

Intune セキュリティ ベースラインは、ユーザーとデバイスを保護するのに役立ちます。 セキュリティ ベースラインは事前構成済みの Windows 設定のグループで、関連するセキュリティ チームが推奨する一連の設定と既定値を適用するために使用されます。 Intune でセキュリティ ベースラインのプロファイルを作成することで、複数のデバイス構成プロファイルで構成されたテンプレートを作成します。

ユーザーやデバイスのグループに対してセキュリティ ベースラインを展開すると、Windows 10 以降のバージョンを実行しているデバイスに設定が適用されます。 たとえば、Microsoft モバイル デバイス管理 (MDM) セキュリティ ベースラインを使用すると、自動的に (1) リムーバブル ドライブに対する BitLocker の有効化、(2) デバイスのロックを解除するためのパスワードの要求、(3) プレーンテキスト認証の無効化が実行されます。 既定値がご利用の環境でうまく機能しない場合には、ベースラインをカスタマイズして必要な設定を適用できます。

セキュリティ ベースラインは、セキュリティで保護されたエンド ツー エンドのワークフローを Microsoft 365 で確立するのにも役立ちます。 この機能には、次のような利点があります。
- セキュリティ ベースラインには、セキュリティに影響を与える設定のベスト プラクティスとおすすめが含まれています。 Intune はグループ ポリシーのベースラインを作成する Windows セキュリティ チームと連携を図っているため、このようなおすすめは正確なガイダンスと豊富な経験に基づいています。
- Intune を使用したことがなく、どこから手を付けたらよいか分からない場合、セキュリティ ベースラインはセキュリティで保護されたプロファイルをすばやく作成して展開するのに役立ちます。
- これらのセキュリティ ベースラインは Intune に組み込まれており、管理に使用できる最先端の機能が含まれています。そのため、現在グループ ポリシーを使用している場合には、セキュリティ ベースラインを使用すると、管理目的で Intune に移行する作業がはるかに簡単になります。

詳細については、「[Windows セキュリティ ベースライン](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines)」および「[モバイル デバイス管理](https://docs.microsoft.com/windows/client-management/mdm/)」を参照してください。