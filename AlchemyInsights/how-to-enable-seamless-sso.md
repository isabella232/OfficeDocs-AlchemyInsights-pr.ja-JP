---
title: シームレスな SSO を有効にする方法
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
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 0659d3fe017d7c77b936d80a308bcb56f94ee322029f79ee095ebeec0b8ea7c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963432"
---
# <a name="how-to-enable-seamless-sso"></a>シームレスな SSO を有効にする方法

シームレスな SSO は、[Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) を使用して有効にします。
  
Azure AD Connect を新規でインストールする場合、[カスタム インストール パス](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)を選択します。**[ユーザー サインイン]** ページで、**[シングル サインオンを有効にする]** オプションを選択します。
  
シームレスな SSO が正しく有効化されたかを確認するには:
  
1. [Azure Active Directory 管理センター](https://aad.portal.azure.com)に全体管理者としてサインインします。

2. 左のウィンドウの **[Azure Active Directory]** を選択します。

3. シームレスなシングル サインオンが **[有効]** になっていることを確認します。

詳細については、[Azure Active Directory シームレス シングル サインオン: クイック スタート](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)に関するページを参照してください。
  