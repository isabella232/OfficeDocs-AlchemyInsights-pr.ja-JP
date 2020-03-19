---
title: Windows 10 で指紋ロック解除オプションを使う
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2020
ms.locfileid: "42592571"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="a528f-102">Windows 10 で指紋ロック解除オプションを使う</span><span class="sxs-lookup"><span data-stu-id="a528f-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="a528f-103">**Windows Hello 指紋認証を有効にする**</span><span class="sxs-lookup"><span data-stu-id="a528f-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="a528f-104">指紋を使用して Windows 10 のロックを解除するには、Windows Hello 指紋認証を設定する必要があります。これには少なくとも 1 本の指を追加 (Windows に登録) します。</span><span class="sxs-lookup"><span data-stu-id="a528f-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="a528f-105">**[設定] > [アカウント] > [サインイン オプション]** に移動します (または[こちら](ms-settings:signinoptions?activationSource=GetHelp)をクリックします)。</span><span class="sxs-lookup"><span data-stu-id="a528f-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="a528f-106">利用可能なサインイン オプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a528f-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="a528f-107">例:</span><span class="sxs-lookup"><span data-stu-id="a528f-107">For example:</span></span>

    ![サインイン オプション。](media/sign-in-options.png)

2. <span data-ttu-id="a528f-109">**[Windows Hello 指紋認証]** をクリックまたはタップし、次に **[設定]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a528f-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="a528f-110">Windows Hello 設定ウィンドウで、**[開始する]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a528f-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="a528f-111">指紋センサーがアクティブになり、このセンサーに指を合わせるように求められます。</span><span class="sxs-lookup"><span data-stu-id="a528f-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![指紋センサー。](media/fingerprint-sensor.png)

3. <span data-ttu-id="a528f-113">指示に従って、指を繰り返しスキャンします。</span><span class="sxs-lookup"><span data-stu-id="a528f-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="a528f-114">これが完了したら、サインインに使用する可能性がある他の指を追加するオプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a528f-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="a528f-115">次回 Windows 10 にサインインするときには、指紋を利用してサインインできます。</span><span class="sxs-lookup"><span data-stu-id="a528f-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="a528f-116">**サインイン オプションとして、Windows Hello 指紋認証が利用できない**</span><span class="sxs-lookup"><span data-stu-id="a528f-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="a528f-117">Windows Hello 指紋認証が**サインイン オプション**に表示されていない場合は、Windows が PC に接続されている指紋リーダーやスキャナーを認識していないか、システム ポリシーがその利用を認めていないということです (たとえば、PC が職場で管理されている場合など)。</span><span class="sxs-lookup"><span data-stu-id="a528f-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="a528f-118">トラブルシューティング:</span><span class="sxs-lookup"><span data-stu-id="a528f-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="a528f-119">タスク バーの **[スタート]** ボタンを選択し、**[デバイス マネージャー]** を探します。</span><span class="sxs-lookup"><span data-stu-id="a528f-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="a528f-120">クリックまたはタップし、**[デバイス マネージャー]** を開きます。</span><span class="sxs-lookup"><span data-stu-id="a528f-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="a528f-121">[デバイス マネージャー] で、シェブロンをクリックして [生体認証デバイス] を展開します。</span><span class="sxs-lookup"><span data-stu-id="a528f-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![生体認証デバイス。](media/biometric-devices.png)

4. <span data-ttu-id="a528f-123">指紋スキャナーが生体認証デバイス (Synaptics WBDI スキャナーなど) に表示されているはずです。</span><span class="sxs-lookup"><span data-stu-id="a528f-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![生体認証デバイス。](media/biometric-devices-expanded.png)

5. <span data-ttu-id="a528f-125">指紋スキャナーが表示されず、スキャナーが PC に統合されている場合は、PC の製造元の Web サイトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a528f-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="a528f-126">PC モデルの [テクニカル サポート] セクションで、インストール可能なスキャナー用の Windows 10 ドライバーを検索します。</span><span class="sxs-lookup"><span data-stu-id="a528f-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="a528f-127">スキャナーが PC と別の場合 (USB で接続されている場合) は、スキャナーの製造元の Web サイトに移動して、使用しているスキャナー モデルの Windows 10 デバイス ドライバー ソフトウェアを見つけてインストールします。</span><span class="sxs-lookup"><span data-stu-id="a528f-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
