---
title: 自動で Microsoft Edge にサインインする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050699"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>自動で Microsoft Edge にサインインする

Microsoft Edge は、OS の既定のアカウントを使用し、ユーザーのデバイス構成に従ってユーザーを自動的にサインインさせます。 

次に、各種類のデバイス構成とそれに依存するユーザー サインイン プロセスのシナリオを以下に説明します。

- **デバイスがハイブリッド/AAD-J の場合**: このオプションは、Windows 10、下位レベルの Windows、および対応するサーバー バージョンで使用できます。 ユーザーは、Azure Active Directory (AD) アカウントで自動的にサインインします。
- **デバイスがドメインに参加している場合**: このオプションは、Windows 10、下位レベルの Windows、および対応するサーバー バージョンで使用できます。 既定では、ドメイン アカウントを持つユーザーは自動的にサインインされません。ユーザーの自動サインインを有効にするには、**ConfigureOnPremisesAccountAutoSignIn** ポリシーを使用します。 Azure AD アカウントを持つユーザーの自動サインインを有効にするには、そのユーザーのデバイスにハイブリッド加入することを検討します。
- **OS の既定のアカウントが Microsoft アカウントである場合**: このオプションは、Windows 10 RS3 (バージョン 1709、ビルド 10.0.16299) 以降のバージョンで使用できます。 このシナリオは、エンタープライズ デバイスではほとんど発生しません。 ただし、OS の既定のアカウントが Microsoft アカウントである場合、Microsoft Edge は自動的に Microsoft アカウントを使用してユーザーをサインインさせます。
 
 
