---
title: フロー認証エラーのトラブルシューティング
ms.author: kaarins
author: kaarins
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: e578149e37c86178b98cf6073f6ed6325f42c455
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393618"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="bd142-102">フロー認証エラーのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="bd142-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="bd142-p101">多くの場合、フローは認証エラーが原因で失敗します。この種類のエラーが発生する場合、エラー メッセージに "権限がありません" と表示されるか、エラー コード 401 または 403 が表示されます。認証エラーは通常、接続を更新することで修正されます。</span><span class="sxs-lookup"><span data-stu-id="bd142-p101">In many cases, flows fail because of an authentication error. If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears. You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="bd142-106">Web ポータルの一番上にある歯車アイコンをクリックまたはタップし、[設定] メニューを開き、[**接続**] をクリックまたはタップします。</span><span class="sxs-lookup"><span data-stu-id="bd142-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="bd142-107">スクロールして、"権限がありません" というエラー メッセージが表示された接続を見つけます。</span><span class="sxs-lookup"><span data-stu-id="bd142-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="bd142-108">接続の横で、接続の未承認に関するメッセージの [**パスワードの確認**] をクリックまたはタップします。</span><span class="sxs-lookup"><span data-stu-id="bd142-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="bd142-109">指示が表示されたら、それに従って資格情報を確認し、フロー実行エラーに戻り、[**再送信**] をクリックまたはタップします。</span><span class="sxs-lookup"><span data-stu-id="bd142-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="bd142-110">詳細については、「[フローのトラブルシューティング](https://go.microsoft.com/fwlink/?linkid=872110)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd142-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

