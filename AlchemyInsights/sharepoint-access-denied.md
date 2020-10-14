---
title: "\"アクセスが拒否されました\" メッセージのトラブルシューティング"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691688"
---
# <a name="troubleshoot-access-denied-messages"></a>"アクセスが拒否されました" メッセージのトラブルシューティング

SharePoint Online のサイトを閲覧しようとしたときにアクセス拒否のメッセージが表示された場合は、次の記事を参照してください。

**ユーザーの追加とライセンス認証**

[一般法人向け Microsoft 365 のユーザーにライセンスが割り当てられている](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)ことを確認してください。

**アクセス許可の割り当て**

ユーザーに SharePoint ライセンスが割り当てられていてもアクセス拒否メッセージが表示される場合は、そのユーザーに[適切なアクセス許可レベルが割り当てられている](https://docs.microsoft.com/sharepoint/understanding-permission-levels)ことを確認してください。

**アクセス要求機能の使用を検討する**

[アクセス要求](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)機能は、ユーザーが表示する権限がないコンテンツへのアクセスを要求できるようにする機能です。 

**カスタム スクリプトの許可がアクセス拒否の問題の原因になることがある**

特定のシナリオでは、「カスタム スクリプトの許可」機能がアクセス拒否の発生原因になります。 影響を受ける機能のリストについては、セキュリティに関する考慮事項と、この機能を無効にする方法に記載されてています。 「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。

注: それまでアクセスできていた複数のユーザーが OneDrive または SharePoint のサイトを利用できない場合は、サービスに一時的な問題が発生している可能性があります。 [サービス正常性ダッシュボードを確認](https://portal.office.com/adminportal/home#/servicehealth)してください。


  

