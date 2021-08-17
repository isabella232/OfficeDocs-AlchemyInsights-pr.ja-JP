---
title: Microsoft Intune セキュリティ ベースラインを使用して Windows 10 デバイスを構成する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: f77fdbb315db8317a6a1374f05489a7f5a0bedcec484dc9ac53a473098583949
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886637"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Microsoft Intune セキュリティ ベースラインを使用して Windows 10 デバイスを構成する

Intune セキュリティ ベースラインは、ユーザーとデバイスを保護するのに役立ちます。 セキュリティ ベースラインは事前構成済みの Windows 設定のグループで、関連するセキュリティ チームが推奨する一連の設定と既定値を適用するために使用されます。 Intune でセキュリティ ベースラインのプロファイルを作成することで、複数のデバイス構成プロファイルで構成されたテンプレートを作成します。

ユーザーやデバイスのグループに対してセキュリティ ベースラインを展開すると、Windows 10 以降を実行するデバイスに設定が適用されます。 たとえば、Microsoft モバイル デバイス管理 (MDM) セキュリティ ベースラインを使用すると、自動的にリムーバブル ドライブに対する BitLocker の有効化、デバイスのロックを解除するためのパスワードの要求、プレーンテキスト認証の無効化が実行されます。 既定値がご利用の環境でうまく機能しない場合には、ベースラインをカスタマイズして必要な設定を適用できます。

セキュリティ ベースラインは、セキュリティで保護されたエンド ツー エンドのワークフローを Microsoft 365 で確立するのにも役立ちます。 セキュリティ ベースラインには、セキュリティに影響を与える設定のベスト プラクティスとおすすめが含まれています。 Intune はグループ ポリシーのベースラインを作成する Windows セキュリティ チームと連携を図っているため、このようなおすすめは正確なガイダンスと豊富な経験に基づいています。

Intune を使用したことがなく、どこから手を付けたらよいか分からない場合、セキュリティ ベースラインはセキュリティで保護されたプロファイルをすばやく作成して展開するのに役立ちます。 セキュリティ ベースラインは Intune に組み込まれており、最先端の管理機能が含まれています。そのため、現在グループ ポリシーを使用している場合は、セキュリティ ベースラインを使用すると、管理目的で Intune に移行する作業がはるかに簡単になります。

詳細については、「[Windows セキュリティ ベースライン](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines)」および「[モバイル デバイス管理](https://docs.microsoft.com/windows/client-management/mdm/)」を参照してください。

