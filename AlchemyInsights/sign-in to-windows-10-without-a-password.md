---
title: パスワードを使用しないで Windows 10 にサインインする
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830551"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>パスワードを使用しないで Windows 10 にサインインする

Windows の起動時にパスワードを入力する必要がないようにするためには、PIN、顔認識、指紋などの Windows Hello の安全なサインイン オプションを使用することをお勧めします。 安全なサインインを無効にするには、以下の「Windows 10 に自動的にサインインする」の手順をご覧ください。

**アカウント パスワードに代わる Windows Hello の安全な代替機能**

**[設定] > [アカウント] > [サインイン オプション]** に移動します (または [こちら](ms-settings:signinoptions?activationSource=GetHelp)をクリックします)。 利用可能なサインイン オプションが表示されます。 例:

![サインイン オプション。](media/sign-in-options.png)

いずれかをクリックまたはタップして、オプションを構成します。 次に Windows を起動またはロック解除するときより、パスワードに代わって新しいオプションを利用できるようになります。 

**Windows 10 に自動的にサインインする**

**注**: 自動サインインは便利ですが、複数の人物が PC にアクセスできる場合は、セキュリティ上のリスクが生じます。 

1. タスクバーの **[スタート]** ボタンをクリックまたはタップします。

2. **netplwiz** と入力して Enter キーを押し、[ユーザー アカウント] ウィンドウを開きます。

3. **[ユーザー アカウント]** で、Windows の起動時に自動的にサインインするアカウントをクリックします。

4. 「ユーザーがこのコンピューターを使うには、ユーザー名とパスワードの入力が必要」のチェックボックスをオフにします。

    ![ユーザーは、ユーザー名とパスワード オプションを入力する必要があります。](media/users-must-enter-username.png)

5. **[OK]** をクリックします。 選択したアカウントのパスワードを入力するように求められます。 **[OK]** をクリックして終了します。 次回 Windows 10 を起動すると、選択したアカウントに自動的にサインインします。
