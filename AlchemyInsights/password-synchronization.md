---
title: パスワード同期
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484083"
---
# <a name="password-synchronization"></a>パスワード同期

[**パスワード ハッシュ同期がまったく動作しない**]

パスワード ハッシュ同期が機能しない場合にお客様が遭遇する一般的な問題は次のとおりです。

- オンプレミスの Active Directory と通信するために Azure AD Connect によって使用される Active Directory アカウントには、**ディレクトリ変更の複製** と **ディレクトリ変更の複製パスワード同期** に必要なすべてのアクセス許可が付与されていません。これらのアクセス許可を Active Directory アカウントに付与して、これを修正する必要があります。
- 管理者がユーザーサインイン方法を **パスワード同期** から Azure AD Connect ウィザードの **AD FS とのフェデレーション** などの別のオプションに変更した後、パスワード ハッシュ同期は無効になります。Azure AD Connect ウィザードで **パスワード ハッシュ同期** 機能を再度有効にすることで、これを修正できます。
- オンプレミスの Active Directory での接続の問題。 たとえば、一部のドメインコントローラーに Azure AD Connect からアクセスできない場合や、[必要なポート](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)がファイアウォールによってブロックされている場合などがあります。Azure AD Connect サーバーとオンプレミスの Active Directory の間の接続が正しく機能することを確認して、これを修正する必要があります。
- Azure AD Connect サーバーは現在ステージング モードになっているため、サーバーはパスワード ハッシュを実行できません。問題のトラブルシューティングを行うには、「[Azure AD Connect 同期を使用したパスワード同期のトラブルシューティング - パスワードが同期されません](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)」セクションで説明されている手順に従います。

[**一部のユーザーでパスワード ハッシュ同期が機能しない**]

1. パスワード ハッシュがユーザーに対して同期されていないことに気付いた場合は、Azure AD Connect の **トラブルシューティング** タスクを使用して、問題を調査し、解決してください。 次のタスクを実行します。

    a. [ウィザードでトラブルシューティング タスクを実行する](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [トラブルシューティング コマンドレットを使用して、特定の用途のパスワード ハッシュ同期の問題を調査します](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. オンプレミスの Active Directory ユーザー オブジェクトで **ユーザーは次回のログオン時にパスワード変更が必要** オプションが有効になっています。 このオプションを有効にすると、ユーザーに一時パスワードが割り当てられ、次回のログオン時にパスワードを変更するように求められます。 Azure AD Connect は、一時パスワードを Azure AD に同期しません。

上記の問題を解決するには、次のいずれかのタスクを実行します。

- オンプレミス アプリケーション (Windows デスクトップなど) にサインインしてパスワードを変更するようにユーザーに依頼します。 新しいパスワードは Azure AD に同期されます。
- **[ユーザーは次回のログオン時にパスワード変更が必要]** オプションを有効にせずに、管理者にユーザーのパスワードを更新してもらい、新しいパスワードをユーザーと共有します。

3. オンプレミスの Active Directory ユーザー オブジェクトが、オブジェクトの同期またはパスワードの同期用に **正しく構成されていません**。 この問題のトラブル シューティングを行うには、「[Azure AD Connect Sync を使用したパスワード ハッシュ同期のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)」で説明されている手順に従います。







