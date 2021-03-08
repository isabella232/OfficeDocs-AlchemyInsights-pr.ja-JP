---
title: ユーザーのプロビジョニング
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484064"
---
# <a name="user-provisioning"></a>ユーザーのプロビジョニング

- [オンデマンド プロビジョニング](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand)機能を使用して、ユーザーをプロビジョニングし、実行された手順に関する詳細な診断を取得します。
- ユーザーとグループのプロビジョニング時に発生する問題のトラブルシューティングについては、トラブルシューティング ガイド「[プロビジョニングされているユーザーがありません](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)」を参照してください。
- ユーザーがプロビジョニングされていないことに気付いた場合は、Azure Active Directory (AD) の「[プロビジョニング ログ (プレビュー)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)」を参照してください。 特定のユーザーに関連するログ エントリを検索します。
- 定期的にプロビジョニングを再開して、前のプロビジョニング サイクルで見落とされたユーザーをキャッチします。
- 当社のサービスにはまだユーザーを評価する機会がないため、ユーザー/グループがプロビジョニングされていない可能性があります。 プロビジョニングに必要な時間と、プロビジョニング構成ページの進行状況バーを確認します。 追加の詳細セクションで指定された一定の状態が、ユーザーが作成/更新/削除された日付より前の場合は、ユーザーがまだ評価されていないことを意味します。 このシナリオでは、プロビジョニング サービスが終了するまで待つ必要があります。 定常状態になっている場合は、Azure ポータルの UI から再起動することをお勧めします。
  - 私たちのサービスは、ソース システム (Azure Active Directory) のユーザー/グループへの変更のみを認識していることに注意してください。 ユーザー/グループがアプリケーション (ServiceNow など) で直接削除された場合、それらの変更は認識されず、ソース システムのユーザーの状態に基づいてロールバックされません。 このシナリオでは、ターゲット アプリケーションで変更を直接ロールバックするのが最善です。
- Microsoft のサービスはユーザー/グループを評価し、プロビジョニングすべきではないと判断しました。
  - 割り当てられたユーザーとグループにスコープを設定した場合は、ユーザー/グループがアプリケーションに割り当てられているかどうかを確認してください。
  - ユーザー/グループがアプリケーションに割り当てられている場合は、それらが既定のアクセス ロールに割り当てられていないことを確認してください。 このロールはプロビジョニングには使用できません。
  - 属性ベースの範囲指定フィルターを設定した場合は、ユーザーが指定した条件を満たしていることを確認してください。
  - ユーザーがターゲット システムに既に存在し、ソースとターゲットのユーザーの状態が一致する場合、それ以上アクションは実行されません。
- サービスはユーザーをプロビジョニングしようとしましたが、失敗しました。 これらのシナリオについては、プロビジョニング ログのトラブルシューティングと推奨事項のタブを確認してください。
  - ユーザーの必須属性が Azure Active Directory にないか、サードパーティ アプリケーションで必要な形式と一致しない可能性があります。 たとえば、ユーザーの Country 属性は、US である必要があるときに United States に設定される場合があります。
  - この属性は、ターゲット アプリケーションにまだ存在しない参照属性です。 参照属性は、グループのメンバーであるユーザーなど、別のオブジェクトを指す属性です。 ユーザーの ID はグループのメンバー属性に含まれますが、それが指すユーザー オブジェクトがすでに存在する場合にのみ処理できます。
