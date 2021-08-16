---
title: SharePoint または OneDrive でアクセスを制限する
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075045"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePoint または OneDrive でアクセスを制限する

SharePoint と OneDrive では、アクセスを許可する必要のあるグループまたは個人にのみアクセス権を付与することにより、ファイル、フォルダー、リストなどのアイテムへのアクセスを制限します。既定では、SharePoint でのアクセス許可は階層内の上位から継承されます。そのため、ファイルのアクセス許可はフォルダーから継承され、フォルダーのアクセス許可はライブラリから継承され、ライブラリのアクセス許可はサイトから継承されます。
  
(サイト全体を共有するなどして) より高いレベルで共有することができますが、サイト上のすべてのアイテムを共有したいわけではない場合は継承設定を解除することもできます。ただし、これは推奨しません。アクセス許可の維持がより複雑になり、将来的に混乱を招くことになるためです。継承設定の解除に代わる可能な方法について説明します。
  
- たとえば、フォルダー内で 1 つのファイルを除くすべてのコンテンツを共有する場合は、その 1 つのファイルを共有されていない新しい場所に移動します。
    
- フォルダーに 2 つのサブフォルダーがある場合、1 つ目のサブフォルダーをグループ A およびグループ B と共有し、かつグループ A のみに 2 つ目のサブフォルダーへのアクセスを許可するには、親フォルダーをグループ A と共有し、1 つ目のサブフォルダーにグループ B を追加します。
    
[ファイルまたはフォルダーの共有を停止する](https://go.microsoft.com/fwlink/?linkid=2008861)
  

