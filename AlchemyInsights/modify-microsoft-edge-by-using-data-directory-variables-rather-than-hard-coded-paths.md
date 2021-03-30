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
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038237"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>ハード コーディングされたパスではなく、データ ディレクトリ変数を使用して Microsoft Edge を変更する

たとえば、Windows では、プロファイル データを既定の場所ではなく、ユーザーのローカル アプリケーション データに格納するには、*UserDataDir* ポリシーを **${local_app_data}\Edge\Profile** に設定します。

詳細については、「[Microsoft Edge ユーザー データ ディレクトリ変数を作成する](https://docs.microsoft.com/deployedge/microsoft-edge-policies)」をご覧ください。