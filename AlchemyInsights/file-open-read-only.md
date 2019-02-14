---
title: 読み取り専用で開いているファイル
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.openlocfilehash: 2b7f27e38412fc2a1dea46027e926c660231ed8b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903065"
---
# <a name="file-open-read-only"></a><span data-ttu-id="4fae6-102">読み取り専用で開いているファイル</span><span class="sxs-lookup"><span data-stu-id="4fae6-102">File open read-only</span></span>

<span data-ttu-id="4fae6-p101">ファイルが開いているときに、それらが読み取り専用で開いていることに気付くことがあります。これは、インターネットからファイルを開くときなどにセキュリティを強化するための場合もあれば、変更可能な設定が原因でそうなっている場合もあります。ここでは、ファイルが読み取り専用で開くいくつかのシナリオとそれを変更するために使用可能な手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="4fae6-p101">You may find that when you are opening files, they open as read-only. In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed. Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="4fae6-106">**ウイルス対策がファイルが読み取り専用で開かれる原因になっている**</span><span class="sxs-lookup"><span data-stu-id="4fae6-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="4fae6-p102">一部のウイルス対策プログラムは、読み取り専用で開くことによって、潜在的に安全でないファイルからユーザーを保護します。これらの設定を調整する方法については、ウイルス対策ソフトウェアのプロバイダーに確認する必要があります。たとえば、BitDefender の「[Bitdefender Control Center でアプリケーションまたはプロセス除外を追加する方法](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl)」に、アプリケーション除外の追加に関する記載があります。</span><span class="sxs-lookup"><span data-stu-id="4fae6-p102">Some antivirus programs may protect you from potentially unsafe files by opening them read-only. You may need to check with your antivirus provider to learn how to adjust these settings. BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="4fae6-110">**ファイルのプロパティが読み取り専用に設定されていないか?**</span><span class="sxs-lookup"><span data-stu-id="4fae6-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="4fae6-p103">ファイルを右クリックして、[プロパティ] を選択することにより、ファイルのプロパティを確認できます。読み取り専用属性がオンになっている場合は、それをオフにして、[OK] をクリックできます。</span><span class="sxs-lookup"><span data-stu-id="4fae6-p103">You can check the file properties by right-clicking on the file and choosing Properties. If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="4fae6-113">**内容が保護ビューに表示されている**</span><span class="sxs-lookup"><span data-stu-id="4fae6-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="4fae6-p104">インターネットやその他の潜在的に安全でない場所からのファイルには、コンピューターを侵害する可能性のあるウイルス、ワーム、またはその他の種類のマルウェアが含まれている可能性があります。これは、メールの添付ファイルやダウンロードしたファイルでもあり得ることです。お使いのコンピューターを保護するために、このような潜在的に安全でない場所からのファイルは保護ビューで開かれます。保護ビューを使用することにより、リスクを軽減しながら、ファイルを読み取って、その内容を表示できます。保護ビューの詳細と設定の変更方法については、記事「[保護ビューとは](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fae6-p104">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer. This is also commonly the case with email attachments or files you've downloaded. To help protect your computer, files from these potentially unsafe locations are opened in Protected View. By using Protected View, you can read a file and see its contents while reducing the risks. For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="4fae6-119">**OneDrive がいっぱいになっていないか?**</span><span class="sxs-lookup"><span data-stu-id="4fae6-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="4fae6-p105">ファイルが OneDrive に保存されており、OneDrive の記憶領域がいっぱいになっている場合は、割り当てられた領域未満になるまで、ドキュメントを保存できません。OneDrive 上の空き領域を確認するには、通知センターで OneDrive アイコンをクリックして、[記憶域の管理 (Manage storage)] を選択するか、[http://onedrive.live.com](http://onedrive.live.com) に移動して、サインインし、画面の左下で使用済み領域の容量を書き留めます。</span><span class="sxs-lookup"><span data-stu-id="4fae6-p105">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space. You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="4fae6-122">**Office はライセンス認証されているか?**</span><span class="sxs-lookup"><span data-stu-id="4fae6-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="4fae6-p106">Office がライセンス認証されていない場合やサブスクリプションの有効期限が切れている場合は、読み取り専用機能制限モードになっている可能性があります。Office をライセンス認証する方法については、「[Office のライセンスのない製品というエラーとアクティブ化のエラー](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fae6-p106">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode. For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="4fae6-125">**他のすべてが失敗する場合**</span><span class="sxs-lookup"><span data-stu-id="4fae6-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="4fae6-126">コンピューターの再起動を試みる</span><span class="sxs-lookup"><span data-stu-id="4fae6-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="4fae6-127">Office の更新プログラムをインストールする</span><span class="sxs-lookup"><span data-stu-id="4fae6-127">Install Office updates</span></span>
    
- <span data-ttu-id="4fae6-128">Office のオンライン修復を実行する</span><span class="sxs-lookup"><span data-stu-id="4fae6-128">Perform an Online repair of Office</span></span>
    

