---
title: コンプライアンス センターでの AIP から MIP/統合ラベル付けへの移行
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674331"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>コンプライアンス センターでの AIP から MIP/統合ラベル付けへの移行

セキュリティ/コンプライアンス センターで AIP ラベルから統合ラベル付けに移行するには、次の手順を実行します。

**Azure ポータルからの保護を有効にする**

1. まだ行っていない場合は、新しいブラウザー ウィンドウを開いて、[Azure ポータルにサインイン](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)します。 **Azure Information Protection** ブレードに移動します。 たとえば、ハブ メニューで [**すべてのサービス**] をクリックし、[フィルタ] ボックスに「**情報**」と入力し始めます。 [**Azure Information Protection**] を選択します。 これまでに Azure Information Protection ブレードにアクセスしたことがない場合は、このブレードをポータルに追加するための 1 回限りの[追加の手順](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)を参照してください。 Azure Information Protection ブレードを開くには、[Azure Information Protection Premium プラン](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)、または Rights Management を含む Office 365 プランが必要です。 これらのサブスクリプションのいずれかを持っているが、有効なサブスクリプションが見つからないというメッセージが表示される場合は、[Microsoft サポートに連絡](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)するか、標準のサポート チャネルを使用してください。

2. [**管理**] メニュー オプションを見つけ、[**保護のアクティブ化**] を選択します。 [**アクティブ化**] をクリックして、操作を確認します。 アクティブ化が完了すると、情報バーに「**アクティブ化は正常に終了しました**」と表示されます。

**Azure Information Protection ラベルを Office 365 セキュリティ/コンプライアンス センターに移行する**

1. グローバル管理者権限を持つユーザーとしてログインしていることを確認してください。

2. **Azure Information Protection** ブレードに移動します。

3. [**管理**] メニュー オプションから [**統合ラベル付け**] を選択します。

4. [**Azure Information Protection - 統合ラベル付け**] ブレードで、[**アクティブ化**] をクリックし、オンラインの指示に従います。

**注**: セキュリティ/コンプライアンス センターの移行をアクティブ化する前に、適切な権限があることを確認してください。 詳細については、次の記事を参照してください。

1. [Azure Information Protection を構成するには、グローバル管理者である必要がありますか、それとも他の管理者に委任できますか?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [セキュリティ/コンプライアンス センターへの移行後の管理者の役割に関する重要な情報。](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

セキュリティ/コンプライアンス センターへの AIP から統合ラベル付けの移行の詳細については、「[ラベルの移行](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)」をご覧ください。
