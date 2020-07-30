---
title: Apple MDM プッシュ証明書が設定されていません
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440571"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="c2d57-102">Apple MDM プッシュ証明書が設定されていません</span><span class="sxs-lookup"><span data-stu-id="c2d57-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="c2d57-103">Apple MDM プッシュ証明書 (Apple Push Notification Service (APNS) 証明書とも呼ばれます) が、お客様のサブスクリプションに構成されていません。</span><span class="sxs-lookup"><span data-stu-id="c2d57-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="c2d57-104">Apple MDM プッシュ証明書が構成されていないと、iOS デバイスや Mac OS デバイスの登録および管理は行えません。</span><span class="sxs-lookup"><span data-stu-id="c2d57-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="c2d57-105">Intune に証明書を追加すると、ユーザーはポータル サイト アプリをインストールして iOS デバイスを登録することができるようになります。</span><span class="sxs-lookup"><span data-stu-id="c2d57-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="c2d57-106">**「同意します。」** を選び</span><span class="sxs-lookup"><span data-stu-id="c2d57-106">Select **"I agree."**</span></span> <span data-ttu-id="c2d57-107">データを Apple に送信するためのアクセス許可を Microsoft に付与します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="c2d57-108">Apple MDM プッシュ証明書の作成に必要な Intune 証明書署名要求を **CSR にダウンロードする** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="c2d57-109">ファイルは、Apple Push Certificates ポータルから信頼関係の証明書を要求するのに使用します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="c2d57-110">**MDM プッシュ証明書を作成する** を選択して、Apple Push Certificates ポータルに移動します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="c2d57-111">会社の Apple ID でサインインし、**証明書を作成する** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="c2d57-112">**ファイルを選ぶ** を選択し、証明書の署名要求ファイルに移動し、**アップロード** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="c2d57-113">確認ページで、**ダウンロード** を選択して証明書 (.pem) ファイルをダウンロードし、ファイルをローカルに保存します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="c2d57-114">**注**: 証明書は、作成に使用された Apple ID に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="c2d57-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="c2d57-115">ベスト プラクティスとして、管理タスクに会社の Apple ID を使用して、メールボックスを複数のユーザーまたは配布リストを使用して監視するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="c2d57-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="c2d57-116">個人用の Apple ID は使用しません。</span><span class="sxs-lookup"><span data-stu-id="c2d57-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="c2d57-117">同じ Apple ID を使用して、12 か月ごとに Apple プッシュ証明書を更新します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="c2d57-118">Apple MDM プッシュ証明書の作成に使用する Apple ID を入力します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="c2d57-119">証明書を更新する必要がある場合のリマインダーとして、この ID を記録します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="c2d57-120">証明書 (.pem) ファイルに移動し、**開く** を選択して、**アップロード** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c2d57-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="c2d57-121">プッシュ証明書を使用して、Intune で Apple デバイスを登録および管理できます。</span><span class="sxs-lookup"><span data-stu-id="c2d57-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>