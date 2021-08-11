---
title: PRT を使用した Microsoft Edge でのシングル サインオン
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
- "9005624"
- "9657"
ms.openlocfilehash: 2980739f3a7c7200ceff5a0f2ed6e913eb06c9c1e60c8eb8b8f102f3f2760f01
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54006967"
---
# <a name="use-prt-based-sso-in-microsoft-edge"></a>PRT を使用した Microsoft Edge でのシングル サインオン

[プライマリ更新トークン (PRT)](https://go.microsoft.com/fwlink/?linkid=2133632) とは、Windows 10、iOS、Android デバイスでの認証に使用される Azure Active Directory キーのことです。 PRT を使用すると、これらのデバイスで使用されるすべてのアプリケーションへのシングル サインオンを実現できます。

Microsoft Edge では、PRT を使用したシングル サインオンへのサポートが元からあり、追加の拡張子は必要はありません。 Windows 10 RS3 以上では、サインインしているユーザーは PRT ベースのシングル サインオンをサポートする Web サイトに、この PRT を使用してシングル サインオンを取得します。
