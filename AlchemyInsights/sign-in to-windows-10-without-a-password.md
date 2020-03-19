---
title: パスワードを使用しないで Windows 10 にサインインする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2020
ms.locfileid: "42592570"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="25245-102">パスワードを使用しないで Windows 10 にサインインする</span><span class="sxs-lookup"><span data-stu-id="25245-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="25245-103">Windows の起動時にパスワードを入力する必要がないようにするためには、PIN、顔認識、指紋などの Windows Hello の安全なサインイン オプションを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="25245-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="25245-104">安全なサインインを無効にするには、以下の「Windows 10 に自動的にサインインする」の手順をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="25245-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="25245-105">**アカウント パスワードに代わる Windows Hello の安全な代替機能**</span><span class="sxs-lookup"><span data-stu-id="25245-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="25245-106">**[設定] > [アカウント] > [サインイン オプション]** に移動します (または[こちら](ms-settings:signinoptions?activationSource=GetHelp)をクリックします)。</span><span class="sxs-lookup"><span data-stu-id="25245-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="25245-107">利用可能なサインイン オプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="25245-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="25245-108">例:</span><span class="sxs-lookup"><span data-stu-id="25245-108">For example:</span></span>

![サインイン オプション。](media/sign-in-options.png)

<span data-ttu-id="25245-110">いずれかをクリックまたはタップして、オプションを構成します。</span><span class="sxs-lookup"><span data-stu-id="25245-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="25245-111">次に Windows を起動またはロック解除するときより、パスワードに代わって新しいオプションを利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="25245-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="25245-112">**Windows 10 に自動的にサインインする**</span><span class="sxs-lookup"><span data-stu-id="25245-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="25245-113">**注**: 自動サインインは便利ですが、複数の人物が PC にアクセスできる場合は、セキュリティ上のリスクが生じます。</span><span class="sxs-lookup"><span data-stu-id="25245-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="25245-114">タスクバーの **[スタート]** ボタンをクリックまたはタップします。</span><span class="sxs-lookup"><span data-stu-id="25245-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="25245-115">**netplwiz** と入力して Enter キーを押し、[ユーザー アカウント] ウィンドウを開きます。</span><span class="sxs-lookup"><span data-stu-id="25245-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="25245-116">**[ユーザー アカウント]** で、Windows の起動時に自動的にサインインするアカウントをクリックします。</span><span class="sxs-lookup"><span data-stu-id="25245-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="25245-117">「ユーザーがこのコンピューターを使うには、ユーザー名とパスワードの入力が必要」のチェックボックスをオフにします。</span><span class="sxs-lookup"><span data-stu-id="25245-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![ユーザーは、ユーザー名とパスワード オプションを入力する必要があります。](media/users-must-enter-username.png)

5. <span data-ttu-id="25245-119">**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="25245-119">Click **OK**.</span></span> <span data-ttu-id="25245-120">選択したアカウントのパスワードを入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="25245-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="25245-121">**[OK]** をクリックして終了します。</span><span class="sxs-lookup"><span data-stu-id="25245-121">Click **OK** to finish.</span></span> <span data-ttu-id="25245-122">次回 Windows 10 を起動すると、選択したアカウントに自動的にサインインします。</span><span class="sxs-lookup"><span data-stu-id="25245-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
