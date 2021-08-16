---
title: MIM 同期サービスを構成する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: f834bead0b6f22dcadc808d45dcefe7f6571ef62c74b7fd97355157ca49542af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978490"
---
# <a name="configure-mim-sync-service"></a>MIM 同期サービスを構成する

Microsoft Identity Manager (MIM) 同期サービスは MIM のコンポーネントです。 これは、複数のオンプレミス ディレクトリとデータベースを持つ組織の情報を保存および統合する一元化されたオンプレミス サービスです。 MIM の最近の更新で問題が解決された場合、または以下のセクションで説明されている他の問題の 1 つである場合は、MIM Sync の問題を解決できる可能性があります。

**推奨される手順**

1. MIM Sync の最新のアップデートを使用していることを確認し、[MIM Sync のリリース ノート](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history)を確認して、アップデートで問題が解決されたかどうかを確認します。
2. 問題が汎用 LDAP、汎用 SQL、Lotus Domino、または Web サービス コネクタにある場合は、[汎用コネクタ](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)の最新の更新を使用していることを確認してください。
3. MIM 同期実行がエラーで停止した場合は、[実行エラーコード](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes)の表を参照して、考えられる原因を特定してください。
4. 実行が **extension-dll-exception** で停止する場合は、それらの単語をクリックして **[コネクタ空間オブジェクト] プロパティ** ウィンドウを開き、**[スタック トレース...]** をクリックして、[Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) で説明されている根本的な原因の詳細を確認します。
5. パスワード変更通知サービス (PCNS) コンポーネントがパスワード同期中にイベント ログに **エラー 6025** を報告する場合は、[エラー 6025 を報告する PCNS](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx) のトラブルシューティング ガイドを確認してください。
6. FIM サービス管理エージェントとの完全同期が遅い場合は、「[遅いまたはハングする完全同期のトラブルシューティング](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)」で説明されているように、TempDB の **自動拡張** 設定を確認してください。
7. FIM サービス管理エージェントを使用して failed-creation-via-web-services で stopped-server のエラーが発生した場合は、原因の概要について、[Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) を参照してください。

