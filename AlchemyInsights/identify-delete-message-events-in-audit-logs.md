---
title: 監査ログのメッセージ イベントの削除を特定する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716501"
---
# <a name="audit-logs-for-deleted-email-messages"></a>削除されたメール メッセージの監査ログ

2019 年 1 月から、Microsoft では、標準でメールボックス監査が有効になっています。 それ以外の場合、特定のユーザーのメッセージの削除を確認するためには、監査の削除操作を手動で有効にする必要があります。 組織または特定のユーザーのメールボックス監査ログが既に有効になっている場合は、次の手順を実行します。

1. [Microsoft 365 セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインします

2. [**検索と調査**] と [**監査ログ検索**]をクリックする。

3. [**開始日付**] と [**終了日付**] フィールドで日付範囲を選択します。 調べたいユーザー(アイテムを削除したユーザー) のユーザー名を指定します。 [**アクティビティ**]フィールドで、[**削除済みアイテム フォルダーからの削除済みメッセージ**] と [**削除済みアイテム フォルダーに移動済みのメッセージ**] を選択します。

4. [**検索**] をクリックします。

結果から、[監査レコード] を選択します。 詳細ポップアップから、 [**詳細情報**]をクリックします。 削除された項目に関する追加情報(件名、項目が削除されたときの場所など) は、 [**対象アイテム**] フィールドに表示されます。 **ClientInfoString** プロパティが、Outlook、Outlook on the web (旧称 Outlook Web App)、またはその他のデバイス上で削除が発生したかどうかを表示します。

詳細については、 [メールボックスへの転送を誰が設定したのか判別する](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)を参照してください。

**注意**: 監査ログ機能を使用して、削除したアイテムを復元することはできません。 Outlook on the web で削除済みのメッセージを取得するには、[Outlook Web App で 削除済みアイテムを復元する](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4) を参照してください。
