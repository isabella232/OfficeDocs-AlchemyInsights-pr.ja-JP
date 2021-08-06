---
title: 902 (重複するオブジェクトに起因する同期エラー)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998799"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>重複するオブジェクトに起因する同期エラー

Microsoft 365 でディレクトリ同期が終了したときに、次のいずれかのエラー メッセージが表示される場合があります。

- Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory. (このオブジェクトに関連付けられた次の属性値はローカル ディレクトリで既に他のオブジェクトに関連付けられているため、Microsoft Online Services でこのオブジェクトを更新できません。)

- 同じプロキシ アドレスを持つ同期済みオブジェクトが Microsoft Online Services ディレクトリ内に既に存在します。

- Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName. (このオブジェクトに関連付けられた属性値 UserPrincipalName は、ローカル ディレクトリ サービスの他のオブジェクトに既に関連付けられているため、このオブジェクトを更新できません。)

問題を特定して修正するには、[IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix) をダウンロードして実行します。

詳細については、「[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)」を参照してください。
