---
title: 読み取り専用ファイルを開く
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: cbc3a97debc70ce7be02f651253c71651bbb2643
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297146"
---
# <a name="file-open-read-only"></a><span data-ttu-id="07a99-102">読み取り専用ファイルを開く</span><span class="sxs-lookup"><span data-stu-id="07a99-102">File open read-only</span></span>

<span data-ttu-id="07a99-p101">ファイルを開くときに開く読み取り専用とすることがあります。場合によっては、これは、セキュリティ強化のために使用する設定を変更できますが、インターネットやその他の時間からファイルを開くときなどです。読み取り専用ファイルを開く場所のいくつかのシナリオと手順を変更するのにはいくつかを次に示します。</span><span class="sxs-lookup"><span data-stu-id="07a99-p101">You may find that when you are opening files, they open as read-only. In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed. Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="07a99-106">**ウイルス対策ソフトウェアが原因とそれらを開くには読み取り専用**</span><span class="sxs-lookup"><span data-stu-id="07a99-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="07a99-p102">ウイルス対策プログラムによって可能性がありますから保護する安全でないファイルが読み取り専用で開きます。これらの設定を調整する方法については、ウイルス対策プロバイダーに確認する必要があります。BitDefender には、たとえば、ここでのアプリケーションの除外を追加する方法の内容が含まれて:[アプリケーションまたは Bitdefender コントロール センターのプロセス除外リストに追加する方法](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl)です。</span><span class="sxs-lookup"><span data-stu-id="07a99-p102">Some antivirus programs may protect you from potentially unsafe files by opening them read-only. You may need to check with your antivirus provider to learn how to adjust these settings. BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="07a99-110">**ファイルのプロパティを設定読み取り専用ですか。**</span><span class="sxs-lookup"><span data-stu-id="07a99-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="07a99-p103">ファイルを右クリックしてプロパティを選択することによって、ファイルのプロパティを確認できます。読み取り専用属性がオンの場合は、オフにし、[OK] をクリックできます。</span><span class="sxs-lookup"><span data-stu-id="07a99-p103">You can check the file properties by right-clicking on the file and choosing Properties. If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="07a99-113">**コンテンツが保護されたビューでは**</span><span class="sxs-lookup"><span data-stu-id="07a99-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="07a99-p104">ウイルス、ワーム、または他の種類のマルウェアがコンピューターに損害を与えることができるインターネットおよびその他の安全でない場所からのファイルを含めることができます。よくの場合は電子メールの添付ファイルまたはダウンロードしたファイルです。お使いのコンピューターを保護するため、これらの安全でない場所からのファイルは保護されたビューで開かれます。保護されたビューを使用すると、ファイルの読み取りし、リスクを削減しながら、内容を確認できます。保護されたビューと設定を変更する方法の詳細については、この資料を参照してください:[保護されたビューとは何ですか?](https://support.office.com/en-us/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="07a99-p104">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer. This is also commonly the case with email attachments or files you've downloaded. To help protect your computer, files from these potentially unsafe locations are opened in Protected View. By using Protected View, you can read a file and see its contents while reducing the risks. For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/en-us/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="07a99-119">**OneDrive がいっぱいですか。**</span><span class="sxs-lookup"><span data-stu-id="07a99-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="07a99-p105">OneDrive に保存されているし、OneDrive の容量がいっぱいに、割り当てられたスペースの下になるまで、文書を保存することはできません。OneDrive では、空き領域をチェックするには通知センターの [OneDrive] アイコンをクリックし、管理のストレージを選択するかに移動することができます[http://onedrive.live.com](http://onedrive.live.com)、サインインし、画面の下で使用される領域の左に注意してください。</span><span class="sxs-lookup"><span data-stu-id="07a99-p105">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space. You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="07a99-122">**Office がアクティブになるでしょうか。**</span><span class="sxs-lookup"><span data-stu-id="07a99-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="07a99-p106">Office がアクティブでない場合、またはサブスクリプションの有効期限が切れている場合は、読み取り専用機能制限モードにすることもできます。Office のライセンス認証方法の詳細についてを参照してください:[ライセンスのない製品と Office のライセンス認証エラー](https://support.office.com/en-us/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380)です。</span><span class="sxs-lookup"><span data-stu-id="07a99-p106">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode. For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/en-us/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="07a99-125">**他のすべてが失敗した場合.**</span><span class="sxs-lookup"><span data-stu-id="07a99-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="07a99-126">コンピューターを再起動してください。</span><span class="sxs-lookup"><span data-stu-id="07a99-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="07a99-127">Office 更新プログラムをインストールします。</span><span class="sxs-lookup"><span data-stu-id="07a99-127">Install Office updates</span></span>
    
- <span data-ttu-id="07a99-128">Office のオンラインの修復を実行します。</span><span class="sxs-lookup"><span data-stu-id="07a99-128">Perform an Online repair of Office</span></span>
    

