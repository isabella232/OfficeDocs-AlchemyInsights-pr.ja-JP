---
title: サービス接続ポイント (SCP) を構成する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038279"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="6665b-102">サービス接続ポイント (SCP) を構成する</span><span class="sxs-lookup"><span data-stu-id="6665b-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="6665b-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="6665b-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="6665b-104">**理由**: SCP オブジェクトを読み取り、Azure AD テナント情報を取得することができない</span><span class="sxs-lookup"><span data-stu-id="6665b-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="6665b-105">**解決**: 「[サービス接続ポイントを構成する](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)」のセクションを参照してください</span><span class="sxs-lookup"><span data-stu-id="6665b-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="6665b-106">**アクション プラン**</span><span class="sxs-lookup"><span data-stu-id="6665b-106">**Action plan**</span></span>

- <span data-ttu-id="6665b-107">制御された検証のために、デバイスが GPO を受信したかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="6665b-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="6665b-108">GPO がレジストリ キーを作成したかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="6665b-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="6665b-109">ディレクトリ ID と onmicrosoft ドメインで作成された 2 つのキーを持っていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="6665b-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="6665b-110">**SCP 用のクライアント側のレジストリ設定を構成する**</span><span class="sxs-lookup"><span data-stu-id="6665b-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="6665b-111">次の例を使用してグループ ポリシー オブジェクト (GPO) を作成し、デバイスのレジストリで SCP エントリを構成するレジストリ設定を展開します。</span><span class="sxs-lookup"><span data-stu-id="6665b-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="6665b-112">グループ ポリシー管理コンソールを開き、ドメインで新しい GPO を作成します。</span><span class="sxs-lookup"><span data-stu-id="6665b-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="6665b-113">新しく作成した GPO の名前を指定します (ClientSideSCP など)</span><span class="sxs-lookup"><span data-stu-id="6665b-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="6665b-114">GPO を編集し、次のパスを見つけます: **[コンピューター構成] > [環境設定] > [Windows 設定] > [レジストリ]**。</span><span class="sxs-lookup"><span data-stu-id="6665b-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="6665b-115">[**レジストリ**] で右クリックし、**[新規] > [レジストリ アイテム]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="6665b-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="6665b-116">[**全般**] タブで、次の内容を構成します。</span><span class="sxs-lookup"><span data-stu-id="6665b-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="6665b-117">**アクション**: 更新</span><span class="sxs-lookup"><span data-stu-id="6665b-117">**Action**: Update</span></span>
    
- <span data-ttu-id="6665b-118">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="6665b-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="6665b-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="6665b-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="6665b-120">**値の名前**: TenantId</span><span class="sxs-lookup"><span data-stu-id="6665b-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="6665b-121">**値の種類**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="6665b-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="6665b-122">**値のデータ**: Azure AD インスタンスの GUID またはディレクトリ ID (この値は、 **[Azure portal] > [Azure Active Directory] > [プロパティ] > [ディレクトリ ID] にあります**)</span><span class="sxs-lookup"><span data-stu-id="6665b-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="6665b-123">**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="6665b-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="6665b-124">[**レジストリ**] で右クリックし、**[新規] > [レジストリ アイテム]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="6665b-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="6665b-125">[**全般**] タブで、次の内容を構成します。</span><span class="sxs-lookup"><span data-stu-id="6665b-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="6665b-126">**アクション**: 更新</span><span class="sxs-lookup"><span data-stu-id="6665b-126">**Action**: Update</span></span>
    
- <span data-ttu-id="6665b-127">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="6665b-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="6665b-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="6665b-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="6665b-129">**値の名前**: TenantName</span><span class="sxs-lookup"><span data-stu-id="6665b-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="6665b-130">**値の種類**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="6665b-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="6665b-131">**値のデータ**: AD FS などのフェデレーション環境を使用している場合は、確認済みのドメイン名です。</span><span class="sxs-lookup"><span data-stu-id="6665b-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="6665b-132">管理環境を使用している場合は、確認済みのドメイン名または onmicrosoft.com ドメイン名 (contoso.onmicrosoft) .com など</span><span class="sxs-lookup"><span data-stu-id="6665b-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="6665b-133">**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="6665b-133">Click **OK**.</span></span>

7. <span data-ttu-id="6665b-134">新しく作成された GPO のエディターを閉じます。</span><span class="sxs-lookup"><span data-stu-id="6665b-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="6665b-135">新しく作成された GPO を、制御されたロールアウト母集団に属するドメインに参加しているコンピューターを含む、目的の OU にリンクします。</span><span class="sxs-lookup"><span data-stu-id="6665b-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="6665b-136">詳細については、「[ハイブリッド Azure AD 参加の制御された検証 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) と[ハイブリッド Azure Active Directory に参加したデバイスのトラブルシューティング | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6665b-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









