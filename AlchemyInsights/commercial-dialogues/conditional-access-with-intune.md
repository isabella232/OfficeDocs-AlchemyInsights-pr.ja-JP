---
title: Intune での条件付きアクセスの使用
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
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005779"
---
# <a name="using-conditional-access-with-intune"></a>Intune での条件付きアクセスの使用

Intune で条件付きアクセスを使用するには、次の 3 つの手順が必要です。

- [コンプライアンス ポリシーを作成して、デバイスが準拠していると見なされるよう満たす必要がある設定を定義します。たとえば、準拠と見なされるには、デバイスには少なくとも 6 桁の暗証番号が必要です。](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [保護されているリソース、およびそれらのリソースにアクセスするために満たす必要がある条件を定義する、条件付きアクセス ポリシーを作成します。たとえば、企業メールにアクセスする前に、デバイスを準拠させる必要があります。](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [コンプライアンス ポリシーと条件付きアクセス ポリシーの両方で、目的のグループのユーザーが対象となるように設定します。これを行うには、Azure Active Directory で特定のユーザー グループを作成する必要がある場合があります。](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[続きを読む](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
