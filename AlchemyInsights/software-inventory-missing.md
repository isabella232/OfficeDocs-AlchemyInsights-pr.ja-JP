---
title: ソフトウェアインベントリが存在しないか不正確です
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: 191d6ae772dc1b1c6b15071da9c4aca14429cf2db17be6ee0db6b23ea0d29e2d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084648"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>ソフトウェアインベントリが存在しないか不正確です

脅威と脆弱性の管理 (TVM) におけるソフトウェア インベントリとは、組織内の既知のソフトウェアを正式な共通プラットフォーム一覧 (CPE)　でリスト化したものです。

公式 CPEのないソフトウェア製品では、脆弱性が公開されません。 また、インベントリには、ベンダー名、弱点の数、脅威、露出しているデバイスの数などの詳細が記載されています。

デバイス上のソフトウェアの変更は、通常 2 時間以内にセキュリティ ポータルに反映されます。 ただし、時間がかかる場合もあります。 現在、強制的に同期させる方法はありません。これは継続的な評価です。

ソフトウェアの変更後、5 時間経過しても TVM に変更が正確に反映されない場合は、以下の手順に従ってください。

1. ソフトウェアがどのように検出されたかについては、ソフトウェア エビデンス セクションを確認してください。
1. ソフトウェアがサポートされているかどうか確認してください。 ソフトウェアは、現在、脅威や脆弱性の管理に対応していなくても、デバイス レベルでしか表示することができない場合があります。 ただし、限られたデータのみ使用可能です。
1. ポータルで誤りを報告する手順については、「[誤りを報告する](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)」を参照してください。
   
    **注**: MDE ポータルでの誤りの報告は、エンジニアリングへの一方通行のチャネルです。 緊急性の高い問題の場合は、サポート チケットを開きます。

詳細については、「[ソフトウェアインベントリ - 脅威と脆弱性の管理](/microsoft-365/security/defender-endpoint/tvm-software-inventory)」を参照してください。