---
title: 既に他のユーザーが組織に Teams をセットアップしていますのエラー
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002343"
- "5063"
ms.openlocfilehash: 5fe3dd4c2cea3b50028b28896c33c8dfe7621a6c0b9fdbee4976dfb0e62c3f5d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909903"
---
# <a name="someone-has-already-set-up-teams-for-your-organization-error"></a>「既に他のユーザーが組織に Teams をセットアップしています」のエラー

Teams で「既に他のユーザーが組織に Teams をセットアップしています」のエラーが表示される場合は、次の原因が考えられます。

1. 他のユーザーが既に Teams を設定しています。招待メールを確認するか、[https://teams.microsoft.com](https://teams.microsoft.com) でドメイン資格情報を使用してプライベート/シークレット Web ブラウザーで Teams にサインインします。

2. 仕事用アカウントと個人用アカウントの両方に関連付けられたメール アドレスでサインインしようとしている。 たとえば、Contoso.com は、Microsoft サービス アカウント (Live ID) と職場アカウント (Active Directory) の両方に使用されます。 この場合、新たなプライベート/incognito ブラウザー ウィンドウで Teams を作成し、サインインの「職場または学校」バージョンを個人バージョンの代わりに選択してください。 それでも問題が解決しない場合は、こうしたリンクを解除し、無料の Teams アカウントを適切に作成する必要があります。 この操作を行うには、「[Microsoft アカウントのメール アドレスまたは電話番号を変更する](https://support.microsoft.com/help/12407)」ページの「サインインに別のアドレスまたは電話番号を使う」にある手順に従います。

3. 現在の仕事用アドレスで無料のテナントにサインアップしようとしている。 この場合、ここでエラーが発生することが予想されます。このアドレスには組織のテナントを使用する必要があります。 [ここ](https://products.office.com/microsoft-teams/group-chat-software)から、個人用メール アドレスを使用して、無料の個人用 Teams アカウントを作成することができます。
