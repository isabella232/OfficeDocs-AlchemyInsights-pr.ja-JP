---
title: Yammer のライセンスに関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148478"
---
# <a name="yammer-licensing-issues"></a>Yammer のライセンスに関する問題

すべてのユーザーは Yammer Enterprise サービスを使用するためにライセンスが必要ですが、既定では、Yammer ではユーザーがサービスにアクセスするためのライセンスを持っている必要はありません。 管理者が Yammer ライセンスのない Microsoft 365 ユーザーをブロックするように設定を変更した場合、Yammer Enterprise のライセンスが割り当てられていないユーザーは、Yammer サービスにアクセスできません。 詳しくは、「[Office 365 で Yammer ユーザー ライセンスを管理する](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)」を参照してください。 

ライセンスがユーザーから削除されると、Yammer タイルは表示されなくなり、他のサービスではライセンスの削除を使って機能を非表示にする可能性があります。 その他の場合、機能は表示されますが、動作するにはライセンスの割り当てが必要になります。  

**ユーザーのライセンスが更新されない**  

ユーザーにライセンスが割り当てられているのに、依然として Yammer にアクセスできない場合があります。 多数のライセンスの割り当てが進行中の場合、遅延が発生する可能性が高くなります。 システムが非同期で実行されているために、Azure AD でライセンスが変更されても、Yammer ユーザーが同じ順序で更新されないことがあります。 ライセンス同期の問題を報告するサポート ケースを開く前に、最大 24 時間待ってください。  

**ライセンスの一括割り当て**  

ライセンスは、管理センターまたは PowerShell スクリプトを使って割り当てることができます。 詳細については、「[ユーザーにライセンスを割り当てる](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)」と「[Office 365 PowerShell を使用してライセンスをユーザー アカウントに割り当てる](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)」を参照してください。 

Microsoft サポートではスクリプトの作成についてのサポートは提供していませんが、Yammer ライセンスの割り当てに関するドキュメントはご利用いただけます。 詳細については、「[Windows PowerShell を使用して Yammer ライセンスを管理する](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)」を参照してください。