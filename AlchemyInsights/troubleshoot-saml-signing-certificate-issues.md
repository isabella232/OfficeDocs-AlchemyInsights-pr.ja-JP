---
title: SAML 署名による証明書の問題のトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: fb043122edf5f99325f0403810eb0dc119d254e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314425"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>SAML 署名による証明書の問題のトラブルシューティング

SAML 署名による証明書の問題を解決するには、次の推奨手順を実行します。

1. SSO をサポートするエンタープライズ アプリケーションを追加すると、Azure は [SAML 署名による証明書](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)と呼ばれる証明書を生成します。 この証明書の有効期限は 3 年です。 証明書の有効期限を変更するには、「 [フェデレーション証明書の有効期限をカスタマイズして、新しい証明書にロール オーバーする](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)」をご覧ください。
2. Azure では、この証明書を使用して、アプリケーションから要求された SAML トークンに署名し、SSO を成功させるためにアプリケーションに送信します。 この手順を完了するには、Azure portal から証明書をダウンロードし、アプリケーション ベンダーに送信して SSO プロセスを完了します。

このプロセスが完了すると、アプリケーションはこの証明書を信頼し、この証明書によって署名された SAML トークンはすべてアプリケーションで承認されます。

3. この証明書の有効期限が切れた場合は、新しい証明書を作成し、アプリケーション ベンダーに更新してから、Azure 側でアクティブにします。 詳細については、「[有効期限が切れそうな証明書を更新する](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)」をご覧ください。

**注**: 証明書の有効期限が切れた場合、ユーザーはブロックされません。

4. 現在の証明書の有効期限が切れる前に、[通知を受信するための電子メールアドレスを追加](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration)します。

**注**: 手順 4 は省略可能です。

5. アプリケーションの SAML 証明書の署名オプションと証明書の署名アルゴリズムを変更します。 詳細については、「[証明書の署名オプションと署名アルゴリズムの変更](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)」をご覧ください。

