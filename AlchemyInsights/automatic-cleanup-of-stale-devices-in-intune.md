---
title: Intune での古いデバイスの自動クリーンアップ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715026"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Intune での古いデバイスの自動クリーンアップ

Intune では、管理者が 90 日から 270 日の間で期間を設定し、この期間を過ぎた場合に古いデバイスがサービスから削除されるように構成できます。 この設定は組織全体に適用され、アクティブになると直ちに有効になります。 設定された期間を超える期間に渡って Intune サーバーにチェックインされなかったデバイスは、完全に削除されます。

**注** このクリーンアップ アクションの対象にできるのは、MDM デバイス オブジェクトのみです。 EAS のみのデバイス オブジェクトは除外されます。

デバイスがデバイスのクリーンアップ設定とその "状態" に基づくデバイス削除の対象になるタイミングの詳細については、次の設定を確認してください。

Setting (設定): **Delete devices after last check-in date (最終チェックイン日の後にデバイスを削除する): Yes (日数の値 (N) が指定されています)**

- デバイスによる最後の正常なチェックインから指定されている日数が経過すると、Intune サービスは設定で構成されている (N) の値を使用してデバイスを削除します。

Setting (設定):  **Delete devices after last check-in date (最終チェックイン日の後にデバイスを削除する): No**

- デバイスの証明書の有効期限が切れてから 180 日経過し、証明書が更新されない場合は、デバイスは削除されます。

**注** いずれの場合も、Intune にデバイスが正常に登録されている必要があります。 登録は、デバイスを初めて Intune サービスにチェックインする際に実行されます。

デバイスが Intune に正常に登録されたにもかかわらず Intune 登録済みとなっていない場合、このデバイスは登録から 270 日後に削除されます。 (デバイスは 90 日後に取消済みとマークされ、それからさらに 180 日後に記録が削除されます。)

Intune コンソールには現在、特定のデバイスのデバイス証明書の有効期限を設定するための機能が備わっていません。