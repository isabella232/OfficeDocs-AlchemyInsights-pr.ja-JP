---
title: エラー コード 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: リモート デスクトップ サービス (RDS) の展開で Office 2013 をアクティブ化中にエラーを発生する場合は、レジストリを編集して ADAL を有効にすることを検討してください。
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499387"
---
リモート デスクトップ サービス (RDS) の展開で Office 2013 をアクティブ化中にエラーを発生する場合は、レジストリを編集して ADAL を有効にすることを検討してください。 
  
|**レジストリ キー**|**タイプ**|**値**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
詳細については、 [Windows デバイスでの Office 2013 の最新認証を有効にする](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)を参照してください。
  
> [!NOTE]
>  ADAL は、Office 365 用リソースおよび 2016 の Office で既定で有効になります。以前 _gt リモート デスクトップ サービス (RDS) ターミナル サービスの名前は。 
  

