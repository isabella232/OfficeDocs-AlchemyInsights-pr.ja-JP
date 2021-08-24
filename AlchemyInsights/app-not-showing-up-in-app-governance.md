---
title: アプリ ガバナンスにアプリが表示されない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/16/2021
ms.locfileid: "58455386"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>アプリ ガバナンスにアプリが表示されない

アプリケーションがアプリ ガバナンスに表示されない場合は、次の内容をチェックします。

1. [Azure AD](https://aad.portal.azure.com/)に移動し、[概要] ページの上部にあるバーでアプリ名を検索してアプリケーションのアプリ ID を検出します。

1. Graph エクスプローラーにアクセスし、このクエリを使用してサービス プリンシパル内のアプリ ID を検索し、<appId> を関連するアプリ ID に置き換えます:  <https://graph.microsoft.com/v1.0/servicePrincipals?$search= "appId:<appId>">

1. 結果が返されない場合は、このクエリを使用してアプリケーション内のアプリ ID を検索し、<appId> を関連するアプリ ID に置き換えます:  <https://graph.microsoft.com/v1.0/applications?$search= "appId:<appId>">

クエリに問題が発生した場合は、「[サポートを受ける](https://docs.microsoft.com/microsoft-365/business-video/get-help-support)」を参照してください。 

アプリ ガバナンスのアプリに関する情報または分析情報に関する詳細については、「[可視性と分析情報に関する詳細情報](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)」を参照してください。

アプリの表示に関する詳細については、「[アプリを表示する](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)」を参照してください。
