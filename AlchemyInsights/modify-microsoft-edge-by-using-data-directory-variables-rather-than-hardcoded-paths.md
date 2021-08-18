---
title: ハードコーディングされたパスではなく、データ ディレクトリ変数を使用して Microsoft Edge を変更する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113421"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>ハードコーディングされたパスではなく、データ ディレクトリ変数を使用して Microsoft Edge を変更する

たとえば、Windows では、プロファイル データを既定の場所ではなく、ユーザーのローカル アプリケーション データに格納するには、**UserDataDir** ポリシーを **${local_app_data}\Edge\Profile** に設定します。 

詳細については、「[Microsoft Edge ユーザー データ ディレクトリ変数を作成する](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)」をご覧ください。