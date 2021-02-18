---
title: グループ ポリシー
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2021
ms.locfileid: "50257015"
---
# <a name="group-policy"></a>グループ ポリシー

Azure Active Directory Domain Services (Azure AD DS) のユーザー オブジェクトとコンピューター オブジェクトの設定は、多くの場合、グループ ポリシー オブジェクト (GPO) を使用して管理されます。 Azure AD DS には、AADDC Users コンテナーおよび AADDC Computers コンテナー用の組み込み GPO が含まれています。 これらの組み込みの GPO をカスタマイズして、環境のニーズに合わせてグループ ポリシーを構成できます。 Azure AD DC 管理者 グループのメンバーは、Azure AD DS ドメイン内でグループ ポリシー管理特権を持っています。また、カスタムの GPO と組織単位 (OU) を作成することもできます。 グループ ポリシーとそのしくみの詳細については、「[グループ ポリシーの概要](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))」を参照してください。

ハイブリッド環境では、オンプレミスの AD DS 環境内で構成されているグループ ポリシーは、Azure AD DS に同期されません。 Azure AD DS のユーザーまたはコンピューターの構成設定を定義するには、既定のいずれかの GPO を編集するか、カスタム GPO を作成します。

こちらの記事「[グループ ポリシーの管理](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy)」では、グループ ポリシー管理ツールのインストール方法、組み込みの GPO の編集方法、カスタム GPO の作成方法について説明します。



