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
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="63ac6-102">パスワードを使用しないで Windows 10 にサインインする</span><span class="sxs-lookup"><span data-stu-id="63ac6-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="63ac6-103">Windows の起動時にパスワードを入力する必要がないようにするためには、PIN、顔認識、指紋などの Windows Hello の安全なサインイン オプションを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="63ac6-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="63ac6-104">安全なサインインを無効にするには、以下の「Windows 10 に自動的にサインインする」の手順をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="63ac6-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="63ac6-105">**アカウント パスワードに代わる Windows Hello の安全な代替機能**</span><span class="sxs-lookup"><span data-stu-id="63ac6-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="63ac6-106">**[設定] > [アカウント] > [サインイン オプション]** に移動します (または [こちら](ms-settings:signinoptions?activationSource=GetHelp)をクリックします)。</span><span class="sxs-lookup"><span data-stu-id="63ac6-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="63ac6-107">利用可能なサインイン オプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="63ac6-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="63ac6-108">例:</span><span class="sxs-lookup"><span data-stu-id="63ac6-108">For example:</span></span>

![サインイン オプション。](media/sign-in-options.png)

<span data-ttu-id="63ac6-110">いずれかをクリックまたはタップして、オプションを構成します。</span><span class="sxs-lookup"><span data-stu-id="63ac6-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="63ac6-111">次に Windows を起動またはロック解除するときより、パスワードに代わって新しいオプションを利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="63ac6-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="63ac6-112">**Windows 10 に自動的にサインインする**</span><span class="sxs-lookup"><span data-stu-id="63ac6-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="63ac6-113">**注**: 自動サインインは便利ですが、複数の人物が PC にアクセスできる場合は、セキュリティ上のリスクが生じます。</span><span class="sxs-lookup"><span data-stu-id="63ac6-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="63ac6-114">タスクバーの **[スタート]** ボタンをクリックまたはタップします。</span><span class="sxs-lookup"><span data-stu-id="63ac6-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="63ac6-115">**netplwiz** と入力して Enter キーを押し、[ユーザー アカウント] ウィンドウを開きます。</span><span class="sxs-lookup"><span data-stu-id="63ac6-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="63ac6-116">**[ユーザー アカウント]** で、Windows の起動時に自動的にサインインするアカウントをクリックします。</span><span class="sxs-lookup"><span data-stu-id="63ac6-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="63ac6-117">「ユーザーがこのコンピューターを使うには、ユーザー名とパスワードの入力が必要」のチェックボックスをオフにします。</span><span class="sxs-lookup"><span data-stu-id="63ac6-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![ユーザーは、ユーザー名とパスワード オプションを入力する必要があります。](media/users-must-enter-username.png)

5. <span data-ttu-id="63ac6-119">**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="63ac6-119">Click **OK**.</span></span> <span data-ttu-id="63ac6-120">選択したアカウントのパスワードを入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="63ac6-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="63ac6-121">**[OK]** をクリックして終了します。</span><span class="sxs-lookup"><span data-stu-id="63ac6-121">Click **OK** to finish.</span></span> <span data-ttu-id="63ac6-122">次回 Windows 10 を起動すると、選択したアカウントに自動的にサインインします。</span><span class="sxs-lookup"><span data-stu-id="63ac6-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
