---
title: Mac での MDATP インストールの問題を解決
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091042"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Mac での MDATP インストールの問題を解決

手動によるインストールに失敗した場合、インストール ウィザードの **サマリー** ページでは次のエラーが表示されます。

"インストール中にエラーが発生しました。 インストーラーでエラーが発生し、インストールに失敗しました。 ソフトウェア製造元にお問い合わせください。"

MDM 展開では、このページに一般的なインストール エラーも表示されます。

エンド ユーザーに正確なエラーは表示されませんが、**/Library/Logs/Microsoft/mdatp/install.log** でインストールの進行状況に関するログ ファイルを保持しています。 このログ ファイルには、各インストール セッションが追加されます。 最後のインストール セッションのみを出力するには、`sed` を使用します。

詳細については、「[Mac 用 Microsoft Defender ATP のインストールの問題を解決](https://go.microsoft.com/fwlink/?linkid=2144615)」を参照します。
