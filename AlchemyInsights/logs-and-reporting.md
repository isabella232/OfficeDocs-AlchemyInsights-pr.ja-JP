---
title: ログとレポーティング
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 03d77c17622a1aac5ecb035bb5b73efdbbfe5e6b141e6b266eef8783f612c8b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067017"
---
# <a name="logs-and-reporting"></a>ログとレポーティング

「[Azure Active Directory レポートに関する FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq)」では、Azure Active Directory (Azure AD) のレポート機能についてよく寄せられる質問への回答をご覧いただけます。 レポートとレポートへのアクセス方法の詳細については、「[Azure Active Directory レポート](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)」を参照してください。

**監査に関する問題のトラブルシューティング**

1. 監査アクティビティの一部が表示される問題が発生し、不足しているアクティビティがこの[リスト](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)に含まれている場合は、サポート チケットを提出してください。
2. テナントで監査ログが表示される問題が発生している場合は、サポート チケットを提出してください。
3. 監査アクティビティがすぐに Azure portal に表示されない場合は「[遅延情報](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)」を確認し、遅延が記載されている遅延時間を超えている場合には、サポート チケットを提出してください。
4. [Azure AD アクティビティ ログの保持](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. 選択した日付の範囲内のすべての監査が表示されない場合は、最大 25 万行 (最新のものから並べ替えて表示) のサインインを Azure portal からダウンロードすることができます。 詳細については、「[Audit activities download (監査アクティビティのダウンロード)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)」を参照してください。

**サインインに関する問題のトラブルシューティング**

1. テナントの Azure AD Premium (P1 または P2) ライセンスを持っている場合のみ、過去 30 日間のデータを表示することができます。
2. サインインは、Azure AD Premium のテナントのみで可能です。 無料ライセンスまたは基本ライセンスのテナントではご利用いただけません。
3. テナントに Premium P1 ライセンスをお持ちにもかかわらずサインインが表示されない場合は「[遅延情報](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)」を確認し、遅延が記載されている遅延時間を超えている場合には、サポート チケットを提出してください。
4. 選択した日付の範囲内のすべてのサインインが表示されない場合は、最大 25 万行 (最新のものから並べ替えて表示) のサインインを Azure portal からダウンロードすることができます。 詳細については、「[Sign-ins activities download (サインイン アクティビティのダウンロード)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)」を参照してください。

**セキュリティ レポートのトラブルシューティング (危険、リスクの高いサインインのフラグが設定されているユーザー)**

1. [リスク セキュリティ レポートのフラグが設定されたユーザー](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Azure Active Directory ポータルのリスクの高いサインイン レポート](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Azure Active Directory リスク イベント](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
