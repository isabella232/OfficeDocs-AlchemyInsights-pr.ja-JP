---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820183"
---
# <a name="blocking-legacy-authentication"></a>レガシ認証のブロック

レガシ認証とは、以下によって行われる認証要求を指す用語です。

- モダンな認証を使用しない、以前のバージョンの Office クライアント (Office 2010 クライアントなど)。

- IMAP/S MTP/POP3 などのレガシ メール プロトコルを使用するクライアント。

レガシ認証のブロックおよびモダンな認証の有効化の詳細については、「[レガシ認証のブロック](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)」を参照してください。

Azure Active Directory (Azure AD) のセキュリティの既定値は、セキュリティの確保を容易にし、組織の保護に貢献します。 セキュリティの既定値には、一般的な攻撃に関する事前構成済みのセキュリティ設定が含まれています。
セキュリティの既定値の詳細については、「[セキュリティの既定値とは](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)」を参照してください。 

**注**: 2019 年 10 月 22 日以降に作成されたテナントの場合、既定でセキュリティ保護されている新しい動作になっており、テナントで既にセキュリティの既定値が有効になっている可能性があります。  すべてのユーザーを保護するために、セキュリティの既定値は、新しく作成されるすべてのテナントに展開されています。
