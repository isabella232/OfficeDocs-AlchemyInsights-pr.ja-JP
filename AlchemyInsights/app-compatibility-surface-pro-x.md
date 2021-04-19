---
title: Microsoft Surface Pro X とのアプリ互換性
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 085815982a3948a7853326541101d2ed21c1869e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837689"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>Microsoft Surface Pro X とのアプリ互換性

Surface Pro X のようなデバイスでは、アプリケーションの実行形態が異なります。ほとんどのアプリには互換性がありますが、いくつかの制限があります。 アプリケーションの実行中に発生する可能性がある問題の一覧を以下に示します。 

**ドライバー。** Windows 10 ARM ベースの PC 用に設計されている場合、ドライバーは動作します。 ドライバーが動作しない場合、アプリまたは依存しているハードウェアも動作しません。 お使いのデバイスに関するその他のサポートについては、「[Windows 10 ARM ベースの PC についてよく寄せられる質問 (FAQ)](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5)」を参照するか、ハードウェアの製造元に問い合わせてください。

**64 ビット (x64) アプリ。** 64 ビット (x64) のアプリは動作しません。 64 ビット (ARM64) アプリ、32 ビット (ARM32) アプリ、または 32 ビット (x86) アプリが必要です。 通常、32 ビット (x86) バージョンのアプリは見つかりますが、一部のアプリ開発者は 64 ビット (x64) アプリのみを提供しています。

**カスタマイズされたアプリ。** 支援技術アプリやクラウド ストレージ アプリなど、Windows の環境をカスタマイズするアプリでは、問題が発生するおそれがあります。 詳細については、アプリケーションの製造元に問い合わせください。

**サード パーティ製のウイルス対策ソフトウェア。** サード パーティ製のウイルス対策ソフトウェアの中にはインストールできないものがあります。 Windows セキュリティは、Windows 10 デバイスのサポートされている有効期間、お客様を保護するのに役立ちます。

**Windows FAX とスキャン。** Windows FAX とスキャンは、Windows 10 ARM ベースの PC では使用できません。

アプリのインストール、アンインストール、または再インストールで問題が発生する場合は、「[アプリのトラブルシューティングの詳細](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details)」を参照してください。

まれなケースを除き、すべてのキーワードは AND ではなく OR である必要があります。