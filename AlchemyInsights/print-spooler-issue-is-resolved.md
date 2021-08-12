---
title: 印刷スプーラーの問題が解決されました
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911343"
---
# <a name="print-spooler-issue-is-resolved"></a>印刷スプーラーの問題が解決されました

使用しているデバイスが Windows 10 **OS Build 19041.329** で更新されていた場合、特定のプリンターで印刷できないという問題が発生している可能性があります。 印刷しようとすると、エラーが発生するか、予期せず終了することがあります。また、プリンターからの出力はありません。 この問題は、OS ビルド **19041.331**、[KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523) で解決されています。  

**調査継続中**

一部のデバイスでは、ローカル セキュリティ機関サブシステム サービス (LSASS) ファイル (**Isass.exe**) が失敗し、次のエラー メッセージが表示されることがあります。「重要なシステム プロセス C:\WINDOWS\system32\Isass.exe に失敗しました (状態コード: c0000008)。 コンピューターを再起動する必要があります。」  **マイクロフトは解決方法に取り組んでおり、今後のリリースで更新プログラムを提供します。**

詳細については、「[Windows 10 Version 2004 に関する既知の問題](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)」を参照してください。