---
title: 属性とスコープ フィルターの問題
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
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484065"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>属性とスコープ フィルターの問題

**競合する UPN 値の問題**

Workday to AD ユーザーのプロビジョニング Workday to AD ユーザーのプロビジョニングは、エラーメッセージ **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique** を表示します。 追加/変更のために提供された UPN 値がフォレスト全体で一意ではないため、操作は失敗しました。 エラーの詳細: **CONSTRAINT_ATT_TYPE - userPrincipalName**。

Workday コネクタ がAD ユーザー アカウントの作成時に設定しようとしている **userPrincipalName** 値は、ターゲット AD ドメインにすでに存在します。 これは、(1) ユーザーがすでに存在し、ユーザーの一致する ID チェックが失敗したか、(2) UPN 生成ルールが競合する値を生成したことを意味します。

推奨される解決手順は次のとおりです。

ユーザーがすでに存在し、一致する ID チェックで Workday アカウントを Active Directory アカウントにリンクできなかった場合は、Workday と AD の両方で一致する ID 属性 (通常は **employeeID**) が完全に一致するかどうかを確認します。 一致するものがない場合は、データの問題を修正する必要があります。 たとえば、Workday の EmployeeID が 001052 で、AD の EmployeeID が 1052 の場合、プロビジョニング エンジンは、2 つのアカウントのリンクに失敗し、既存のユーザーを作成しようとします。 この場合は、AD の **EmployeeID** 値を変更して、先行のゼロを含めて 001052 にすることで解決できます。
UPN 生成式が一意の値を生成していない場合は、重複排除関数 **SelectUniqueValue** を使用して、毎回一意の値を生成することを検討してください。

**Workday to AD User Provisioningは、AD ユーザー アカウントのマネージャー属性値を設定しません**

Workday to AD User Provisioning ジョブは、AD ユーザー アカウントの **マネージャー** 属性値を設定していません。 この動作が見られる場合、次の 2 つのシナリオが考えられます。

1. Manager がスコープ内にないため、Workday のマネージャーに対応する AD ユーザー アカウントに解決できません。
2. **複数の AD ドメイン** のシナリオでは、Workday のマネージャーはユーザーと同じドメインに存在しません。

問題を解決するには、次の手順を試してください。

1. スコープ フィルターを定義した場合は、最初にマネージャーがスコープ内にあるかどうか、およびマネージャーがスコープ句を満たしているかどうかを確認します。 マネージャがスコープ フィルターを満たさない場合は、フィルタを変更して、マネージャもプロビジョニング操作の範囲内にあるようにします。
2. 複数の AD ドメインがある場合、コネクタには、クロス ドメイン マネージャー参照を解決できないという既知の制限があります。

自動プロビジョニング用の Workday の構成の詳細については、「[チュートリアル: Workday を構成し、自動ユーザー プロビジョニングに対応させる](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)」を参照してください。













