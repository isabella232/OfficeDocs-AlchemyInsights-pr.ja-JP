---
title: Intune Exchange オンプレミス コネクタ
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808230"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange オンプレミス コネクタ

オンプレミスでホストされている Intune と Exchange との間にコネクタを設定する方法の詳細については、次の文書を参照してください。

[Microsoft Intune Azure でオンプレミスの Intune Exchange コネクタを設定する](https://docs.microsoft.com/intune/exchange-connector-install)

**よくあるご質問:**

Q: Exchange コネクタを設定しようとすると、"Exchange Connector バージョンがサポートされていません" のようなエラーが表示されます。 何が原因なのでしょうか?

A: ご使用のアカウントには適切にライセンスが割り当てられています。アクティブな Intune ライセンスが必要です。

Q: 複数の Exchange コネクタを所有することはできますか?

A: それぞれの Exchange 組織に存在する Intune テナントごとに 1 つのExchange コネクタのみ設定できます。 コネクタは、マルチ サーバーの Exchange 組織にある 1 つのサーバーにのみインストールできます。

また、同じテナントに構成されているオンプレミスの Exchange と Exchange Online の両方のコネクタを構成することはできません。

Q: コネクタでは、CAS 配列を Exchange への接続として使用することはできますか?

A: CAS 配列の指定は、コネクタ設定でサポートされている構成ではありません。 指定できるサーバーは 1 つのみで、次で検索できるコネクタ構成ファイルにハードコーディングされている必要があります。

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

次のエントリ ```<ExchangeWebServiceURL />``` を検索して、URL を Exchange サーバーに置き換えます。

**例:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

その他のトラブルシューティングについては、次の文書を参照してください。[Intune オンプレミス Exchange コネクタのトラブルシューティング](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Exchange コネクタの詳細ログを有効にする**

1. 編集用に Exchange コネクタ Tracing 構成ファイルを開きます。  
このファイルは次の場所にあります: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**例:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. 次のキーを使用して TraceSourceLine を検索します。OnPremisesExchangeConnectorService  
  
3. SourceLevel ノード値を Information ActivityTracing (既定) から Verbose ActivityTracing に変更する  

**例:** 
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Microsoft Intune Exchange サービスを再起動する  
5. Intune ポータルの完全な同期が完了してから XML を "Information ActivityTracing" に戻し、Microsoft Intune Exchange サービスを再起動します。  
6. ログの場所は次のとおりです。`%ProgramData%\Microsoft\Windows Intune Exchange Connector`