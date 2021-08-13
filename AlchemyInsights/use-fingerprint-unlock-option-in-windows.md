---
title: Windows 10 で指紋ロック解除オプションを使う
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
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971940"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Windows 10 で指紋ロック解除オプションを使う

**Windows Hello 指紋認証を有効にする**

指紋を使用して Windows 10 のロックを解除するには、Windows Hello 指紋認証を設定する必要があります。これには少なくとも 1 本の指を追加 (Windows に登録) します。 

1. **[設定] > [アカウント] > [サインイン オプション]** に移動します (または [こちら](ms-settings:signinoptions?activationSource=GetHelp)をクリックします)。 利用可能なサインイン オプションが表示されます。 例:

    ![サインイン オプション。](media/sign-in-options.png)

2. **[Windows Hello 指紋認証]** をクリックまたはタップし、次に **[設定]** をクリックします。 Windows Hello 設定ウィンドウで、**[開始する]** をクリックします。 指紋センサーがアクティブになり、このセンサーに指を合わせるように求められます。

   ![指紋センサー。](media/fingerprint-sensor.png)

3. 指示に従って、指を繰り返しスキャンします。 これが完了したら、サインインに使用する可能性がある他の指を追加するオプションが表示されます。 次回 Windows 10 にサインインするときには、指紋を利用してサインインできます。

**サインイン オプションとして、Windows Hello 指紋認証が利用できない**

Windows Hello 指紋認証が **サインイン オプション** に表示されていない場合は、Windows が PC に接続されている指紋リーダーやスキャナーを認識していないか、システム ポリシーがその利用を認めていないということです (たとえば、PC が職場で管理されている場合など)。 トラブルシューティング: 

1. タスク バーの **[スタート]** ボタンを選択し、**[デバイス マネージャー]** を探します。

2. クリックまたはタップし、**[デバイス マネージャー]** を開きます。

3. [デバイス マネージャー] で、シェブロンをクリックして [生体認証デバイス] を展開します。

   ![生体認証デバイス。](media/biometric-devices.png)

4. 指紋スキャナーが生体認証デバイス (Synaptics WBDI スキャナーなど) に表示されているはずです。

   ![生体認証デバイス。](media/biometric-devices-expanded.png)

5. 指紋スキャナーが表示されず、スキャナーが PC に統合されている場合は、PC の製造元の Web サイトを参照してください。 PC モデルの [テクニカル サポート] セクションで、インストール可能なスキャナー用の Windows 10 ドライバーを検索します。

6. スキャナーが PC と別の場合 (USB で接続されている場合) は、スキャナーの製造元の Web サイトに移動して、使用しているスキャナー モデルの Windows 10 デバイス ドライバー ソフトウェアを見つけてインストールします。
