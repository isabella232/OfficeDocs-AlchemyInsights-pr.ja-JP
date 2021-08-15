---
title: 単一ユーザーの問題
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
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960156"
---
# <a name="problem-with-single-user"></a>単一ユーザーの問題

- サービスがまだユーザーを評価する機会を与えていないため、ユーザーがプロビジョニングされていない可能性があります。 プロビジョニングに必要な時間と、プロビジョニング構成ページの進行状況バーを確認します。 追加の詳細セクションで指定された一定の状態が、ユーザーが作成/更新/削除された日付より前の場合は、ユーザーがまだ評価されていないことを意味します。 このシナリオでは、プロビジョニング サービスが終了するまで待つ必要があります。

  - サービスは、ソース システム (クラウド HR) 内のユーザーに対する変更のみを認識している点に注意してください。 Azure AD が変更を検出して Active Directory に流し込むには、Azure AD のソース システムに有効な変更が必要です。
- プロビジョニング サービスによってユーザーが評価され、プロビジョニングできないと判断されました。
  - 属性ベースの範囲指定フィルターを設定した場合は、ユーザーが指定した条件を満たしていることを確認してください。
  - ユーザーがターゲット システムに既に存在し、ソースとターゲットのユーザーの状態が一致する場合、それ以上アクションは実行されません。
- プロビジョニング サービスがユーザーのプロビジョニングを試みましたが、失敗しました。 これらのシナリオでは、プロビジョニング ログの「トラブルシューティングと推奨事項」タブを確認します。
  - オンプレミスの Active Directory または Azure AD に、ユーザーの必須属性がない可能性があります。 たとえば、userPrincipalName または sAMAccountName 生成ルールが正しい値を生成していないとします。
  - 一致する属性 (通常は employeeId) は、オンプレミスの Active Directory または Azure AD の一意のユーザーに対して解決されません。 たとえば、AD で同じ employeeId を持つユーザーが 2 人いて、サービスが同じソース エントリの重複対象エントリを示すエラー コードを返しているとします。

単一のユーザーとグループのログを確認するには、「[特定のユーザーグループに関する問題のプロビジョニング ログを確認する](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)」を参照してください。
