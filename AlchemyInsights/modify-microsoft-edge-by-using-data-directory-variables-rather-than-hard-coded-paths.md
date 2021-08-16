---
title: ハード コーディングされたパスではなく、データ ディレクトリ変数を使用して Microsoft Edge を変更する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: e3ad930ec79ef82f3bf95e84cb88e8bb9aea13637d8e59d845b486604664b137
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53992296"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>ハード コーディングされたパスではなく、データ ディレクトリ変数を使用して Microsoft Edge を変更する

たとえば、Windows では、プロファイル データを既定の場所ではなく、ユーザーのローカル アプリケーション データに格納するには、*UserDataDir* ポリシーを **${local_app_data}\Edge\Profile** に設定します。

詳細については、「[Microsoft Edge ユーザー データ ディレクトリ変数を作成する](https://docs.microsoft.com/deployedge/microsoft-edge-policies)」をご覧ください。