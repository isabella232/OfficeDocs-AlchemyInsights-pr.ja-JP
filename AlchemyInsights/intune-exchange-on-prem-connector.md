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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="96f26-102">Intune Exchange オンプレミス コネクタ</span><span class="sxs-lookup"><span data-stu-id="96f26-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="96f26-103">オンプレミスでホストされている Intune と Exchange との間にコネクタを設定する方法の詳細については、次の文書を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96f26-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="96f26-104">Microsoft Intune Azure でオンプレミスの Intune Exchange コネクタを設定する</span><span class="sxs-lookup"><span data-stu-id="96f26-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="96f26-105">**よくあるご質問:**</span><span class="sxs-lookup"><span data-stu-id="96f26-105">**FAQ:**</span></span>

<span data-ttu-id="96f26-106">Q: Exchange コネクタを設定しようとすると、"Exchange Connector バージョンがサポートされていません" のようなエラーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="96f26-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="96f26-107">何が原因なのでしょうか?</span><span class="sxs-lookup"><span data-stu-id="96f26-107">What could be the cause?</span></span>

<span data-ttu-id="96f26-108">A: ご使用のアカウントには適切にライセンスが割り当てられています。アクティブな Intune ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="96f26-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="96f26-109">Q: 複数の Exchange コネクタを所有することはできますか?</span><span class="sxs-lookup"><span data-stu-id="96f26-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="96f26-110">A: それぞれの Exchange 組織に存在する Intune テナントごとに 1 つのExchange コネクタのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="96f26-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="96f26-111">コネクタは、マルチ サーバーの Exchange 組織にある 1 つのサーバーにのみインストールできます。</span><span class="sxs-lookup"><span data-stu-id="96f26-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="96f26-112">また、同じテナントに構成されているオンプレミスの Exchange と Exchange Online の両方のコネクタを構成することはできません。</span><span class="sxs-lookup"><span data-stu-id="96f26-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="96f26-113">Q: コネクタでは、CAS 配列を Exchange への接続として使用することはできますか?</span><span class="sxs-lookup"><span data-stu-id="96f26-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="96f26-114">A: CAS 配列の指定は、コネクタ設定でサポートされている構成ではありません。</span><span class="sxs-lookup"><span data-stu-id="96f26-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="96f26-115">指定できるサーバーは 1 つのみで、次で検索できるコネクタ構成ファイルにハードコーディングされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="96f26-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="96f26-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="96f26-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="96f26-117">次のエントリ ```<ExchangeWebServiceURL />``` を検索して、URL を Exchange サーバーに置き換えます。</span><span class="sxs-lookup"><span data-stu-id="96f26-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="96f26-118">**例:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="96f26-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="96f26-119">その他のトラブルシューティングについては、次の文書を参照してください。[Intune オンプレミス Exchange コネクタのトラブルシューティング](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="96f26-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="96f26-120">**Exchange コネクタの詳細ログを有効にする**</span><span class="sxs-lookup"><span data-stu-id="96f26-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="96f26-121">編集用に Exchange コネクタ Tracing 構成ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="96f26-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="96f26-122">このファイルは次の場所にあります: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="96f26-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="96f26-123">**例:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="96f26-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="96f26-124">次のキーを使用して TraceSourceLine を検索します。OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="96f26-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="96f26-125">SourceLevel ノード値を Information ActivityTracing (既定) から Verbose ActivityTracing に変更する</span><span class="sxs-lookup"><span data-stu-id="96f26-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="96f26-126">**例:** </span><span class="sxs-lookup"><span data-stu-id="96f26-126">**Example:**</span></span>
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
4. <span data-ttu-id="96f26-127">Microsoft Intune Exchange サービスを再起動する</span><span class="sxs-lookup"><span data-stu-id="96f26-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="96f26-128">Intune ポータルの完全な同期が完了してから XML を "Information ActivityTracing" に戻し、Microsoft Intune Exchange サービスを再起動します。</span><span class="sxs-lookup"><span data-stu-id="96f26-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="96f26-129">ログの場所は次のとおりです。`%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="96f26-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>