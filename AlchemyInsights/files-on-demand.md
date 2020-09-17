---
title: ファイル オンデマンド
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804419"
---
# <a name="configure-files-on-demand"></a>ファイル オンデマンドを構成する

OneDrive ファイル オンデマンド機能を利用すれば、OneDrive のファイルをすべてダウンロードし、デバイス上の記憶域を使用することなく、すべてのファイルにアクセスできるようになります。

PC でファイル オンデマンドを構成するには:

1. Windows タスク バーの通知領域で、白または青の **OneDrive** クラウドのアイコンを選択します。 [**ヘルプと設定**] の歯車アイコン、[**設定**] の順に選択します。
2. [**設定**] タブで、[**容量を節約し、ファイルを使用するときにダウンロード**] ボックスをオンにします。  

レジストリを使用してファイル オンデマンドを構成することもできます。

この設定を無効にした場合は、Windows 10 ユーザーは、以前のバージョンの Windows ユーザーと同じ同期動作となり、ファイル オンデマンドを有効にすることはできません。 この設定を構成しなかった場合、ユーザーは、ファイル オンデマンドをオンまたはオフにすることができます。

このポリシーを有効にすると、次のレジストリ キー値が 1 に設定されます。 このポリシーを無効にすると、次のレジストリ キーの値が 0 にセットされます。

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

[設定] に [ファイル オンデマンド] オプションが表示されない場合は、サービスの [Windows クラウドのファイル フィルター ドライバー] の開始の種類が 2 (AUTO_START) に設定されていることを確認してください。 このポリシーを有効にすると、次のレジストリ キー値が 2 に設定されます。

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`