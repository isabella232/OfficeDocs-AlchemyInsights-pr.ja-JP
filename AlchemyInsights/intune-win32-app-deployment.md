---
title: Intune Win32 アプリの展開
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/06/2020
ms.locfileid: "48462089"
---
# <a name="intune-win32-app-deployment"></a>Intune Win32 アプリの展開

Microsoft Intune では、MSI や .EXE を含むもののこれらに限定されない Win32 アプリケーションを Windows 10 デバイスに展開することができます。 使用されている展開メカニズムでは、対象デバイスに Intune 管理拡張機能 (IME) が存在する必要があります。 IME は、PowerShell スクリプトまたは win32 アプリケーションの展開をユーザー/デバイスに対象設定すると、自動的にインストールされます。

また、以下を含む Win32 アプリを展開するために満たす必要がある前提条件のセットも用意されています。

- サポートされているプラットフォーム: Windows 10 バージョン 1607 以降 (エンタープライズ、プロ、教育バージョン)。
- サポートされているアーキテクチャ: x86 と x64。
- デバイスの管理: AAD 参加と自動登録 (ハイブリッド ドメイン参加やグループ ポリシーの自動登録を含む)。
- アプリケーション パッケージの形式: [Microsoft Win32 コンテンツ準備ツール](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)によって準備された .**intunewin** ファイル。
- 制限事項:
    - 最大サイズ: 8GB。
    - サポートされていないアーキテクチャ: ARM。

これらの手順に関連する情報については、ドキュメント「[Add, assign, and monitor a Win32 app in Microsoft Intune (Microsoft Intune での Win32 アプリの追加、割り当て、監視)](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)」を参照してください。

Win32 アプリを含む Windows でのアプリケーションの展開のトラブルシューティングに関する詳細情報については、以下のドキュメントを参照してください

- [アプリのインストールに関する問題のトラブルシューティング](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Win32 アプリのトラブルシューティング](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)