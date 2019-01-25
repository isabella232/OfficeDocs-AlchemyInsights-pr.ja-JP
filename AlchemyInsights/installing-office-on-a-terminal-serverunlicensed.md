---
title: ターミナル サーバーのライセンスで office をインストールします。
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477109"
---
# <a name="installing-office-on-a-terminal-server"></a>ターミナル サーバーに Office をインストールします。

Office 365 用リソースのリモート デスクトップ サービス (RDS) を使用して、Windows サーバーを展開する、以前という名前のターミナル サービス。
  
- Office 365 用リソース、Office 365 エンタープライズ E3、E5 の企業などを含む、Office 365 のプランが必要です。Office 365 のビジネスと Office 365 のビジネス プレミアム プランは、Office 365 用リソースに含めないでください。
    
- [共有のコンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。
    
Office 365 ポータルから RDS に、Office 365 用リソースをインストールする場合は、* **既定のインストール設定を使用する** *、これらの手順に従います。 
  
1. あるどのような Office 365 のプランを確認してください。[についてはどのように](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. 必要に応じて、別の Office 365 に切り替える予定がある場合。[についてはどのように](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. 場合は、他の Office 365 のプランを使用して RDS サーバーには、Office が既にインストールされて、それをアンインストールします。コントロール パネルで、\>プログラムをアンインストールします。問題が発生している場合は、[マイクロソフトのサポートと回復時のアシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールします。 
    
4. RDS サーバーで、管理者アカウントと[Office 365 用リソースのインストール](https://portal.office.com/OLS/MySoftware.aspx)と Office 365 ポータルにサインインします。
    
5. Office をインストールすると、* **を開くまたはにサインインしない** * すべての Office アプリケーションにします。 
    
6. RDS サーバーで、次の手順でレジストリを編集することによって共有されているコンピューターのライセンス認証を有効にします。
    
1. 画面の左下隅の [Windows] ボタンを右クリックし、[実行] を選択します。[名前] ボックスに**regedit**と入力し、[ok] を選択します。 
    
2. 選択 [はい] レジストリ エディターを許可するメッセージが表示されたら、デバイスを変更するのにします。
    
3. レジストリ エディターでは、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration の下に 1 を設定すると**SharedComputerLicensing**の文字列値を追加します。 
    
7. RDS サーバーでは、* * *、エンド ・ ユーザーとしてサインイン** * [Office 365 用リソースの共有のコンピューターのライセンス認証が有効になっている](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)ことを確認します。
    
前提条件、セットアップ方法について説明し、このガイドには、Office の展開ツールを使用してインストールをカスタマイズの詳細についてを参照してください[展開 Office 365 用リソースがリモート デスクトップ サービスを使用して](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)ください。
  
共有のコンピューターのライセンス認証に関連するエラーを修正するのには、 [Office 365 用リソースの共有のコンピューターのライセンス認証の問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)を参照してください。
  

