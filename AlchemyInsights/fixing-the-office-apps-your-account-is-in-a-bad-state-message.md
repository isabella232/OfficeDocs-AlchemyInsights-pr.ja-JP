---
title: Office アプリのアカウントの状態が正しくありません。エラーを修正する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886880"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="fac14-102">Office アプリの "アカウントの状態が正しくありません。" エラーを修正する</span><span class="sxs-lookup"><span data-stu-id="fac14-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="fac14-103">このエラーを修正するには、影響を受けているコンピューター上で以下のオプションを試してみてください。</span><span class="sxs-lookup"><span data-stu-id="fac14-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="fac14-104">Office アプリを開き、[**ファイル**] > [**アカウント**] > [**すべてのアカウントからサインアウト**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fac14-104">Open an Office app, select File  Account, and sign out of all accounts.</span></span> <span data-ttu-id="fac14-105">ライセンスが有効なユーザー アカウントを使用して、もう一度サインインします。</span><span class="sxs-lookup"><span data-stu-id="fac14-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="fac14-106">詳細については、「[Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fac14-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="fac14-107">Windows 資格情報マネージャーを使用して、[Office の資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。</span><span class="sxs-lookup"><span data-stu-id="fac14-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="fac14-108">**注:** Office 2016 のレジストリ パスは 16.0 に変更されています。</span><span class="sxs-lookup"><span data-stu-id="fac14-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="fac14-109">たとえば、\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="fac14-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="fac14-110">影響を受けるコンピューター上で、次の手順に従い EnableADAL = 0 を設定します。</span><span class="sxs-lookup"><span data-stu-id="fac14-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="fac14-111">[Windows] ボタンを右クリックし、[**実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fac14-111">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="fac14-112">[**名前**] ボックスに **regedit** と入力し、[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fac14-112">In the Open box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="fac14-113">レジストリ エディターがデバイスに変更を加えられるようにするかどうかを尋ねるプロンプトが表示されたら、[**はい**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fac14-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="fac14-114">レジストリ エディターで、HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity の下に EnableADAL の DWORD 値を 0 の設定で追加します。</span><span class="sxs-lookup"><span data-stu-id="fac14-114">In Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="fac14-115">Office 2013 を使用して Office 365 に接続している最中にエラーが発生した場合には、Office クライアントの[モダンな認証を有効](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)にします。</span><span class="sxs-lookup"><span data-stu-id="fac14-115">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="fac14-116">詳細については、「[How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune (Office 365、Azure、または Intune にサインインできない非ブラウザー アプリのトラブルシューティング)](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fac14-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

