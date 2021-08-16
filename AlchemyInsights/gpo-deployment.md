---
title: GPO 展開
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067845"
---
# <a name="gpo-deployment"></a>GPO 展開

Azure Active Directory Domain Services (Azure AD DS) のユーザー オブジェクトとコンピューター オブジェクトの設定は、多くの場合、グループ ポリシー オブジェクト (GPO) を使用して管理されます。 Azure AD DS には、AADDC Users コンテナーおよび AADDC Computers コンテナー用の組み込み GPO が含まれています。 これらの組み込みの GPO をカスタマイズして、環境のニーズに合わせてグループ ポリシーを構成できます。 Azure AD DC 管理者 グループのメンバーは、Azure AD DS ドメイン内でグループ ポリシー管理特権を持っています。また、カスタムの GPO と組織単位 (OU) を作成することもできます。 グループ ポリシーとそのしくみの詳細については、「[グループ ポリシーの概要](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))」を参照してください。

ハイブリッド環境では、オンプレミスの AD DS 環境内で構成されているグループ ポリシーは、Azure AD DS に同期されません。 Azure AD DS のユーザーまたはコンピューターの構成設定を定義するには、既定のいずれかの GPO を編集するか、カスタム GPO を作成します。

こちらの記事「[グループ ポリシーの管理](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy)」では、グループ ポリシー管理ツールのインストール方法、組み込みの GPO の編集方法、カスタム GPO の作成方法について説明します。
