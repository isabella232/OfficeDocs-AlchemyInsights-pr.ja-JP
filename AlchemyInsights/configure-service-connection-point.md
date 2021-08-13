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
ms.openlocfilehash: 5ccb55996ccef4b55c8d80de6e35f4ba27e3dfa18dfcaeaf6f6ad1c54b6bb376
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965970"
---
# <a name="configure-service-connection-point-scp"></a>サービス接続ポイント (SCP) を構成する

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **理由**: SCP オブジェクトを読み取り、Azure AD テナント情報を取得することができない
- **解決**: 「[サービス接続ポイントを構成する](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)」のセクションを参照してください


**アクション プラン**

- 制御された検証のために、デバイスが GPO を受信したかどうかを確認します。
- GPO がレジストリ キーを作成したかどうかを確認します。
- ディレクトリ ID と onmicrosoft ドメインで作成された 2 つのキーを持っていることを確認します。

**SCP 用のクライアント側のレジストリ設定を構成する**

次の例を使用してグループ ポリシー オブジェクト (GPO) を作成し、デバイスのレジストリで SCP エントリを構成するレジストリ設定を展開します。

1. グループ ポリシー管理コンソールを開き、ドメインで新しい GPO を作成します。
     - 新しく作成した GPO の名前を指定します (ClientSideSCP など)

2. GPO を編集し、次のパスを見つけます: **[コンピューター構成] > [環境設定] > [Windows 設定] > [レジストリ]**。

3. [**レジストリ**] で右クリックし、**[新規] > [レジストリ アイテム]** の順に選択します。

4. [**全般**] タブで、次の内容を構成します。
  
- **アクション**: 更新
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **値の名前**: TenantId
    
- **値の種類**: REG_SZ
    
- **値のデータ**: Azure AD インスタンスの GUID またはディレクトリ ID (この値は、 **[Azure portal] > [Azure Active Directory] > [プロパティ] > [ディレクトリ ID] にあります**)
 
- **[OK]** をクリックします。
 
5. [**レジストリ**] で右クリックし、**[新規] > [レジストリ アイテム]** の順に選択します。

6. [**全般**] タブで、次の内容を構成します。
  
- **アクション**: 更新
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **値の名前**: TenantName
    
- **値の種類**: REG_SZ
    
- **値のデータ**: AD FS などのフェデレーション環境を使用している場合は、確認済みのドメイン名です。 管理環境を使用している場合は、確認済みのドメイン名または onmicrosoft.com ドメイン名 (contoso.onmicrosoft) .com など

- **[OK]** をクリックします。

7. 新しく作成された GPO のエディターを閉じます。

8. 新しく作成された GPO を、制御されたロールアウト母集団に属するドメインに参加しているコンピューターを含む、目的の OU にリンクします。

詳細については、「[ハイブリッド Azure AD 参加の制御された検証 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) と[ハイブリッド Azure Active Directory に参加したデバイスのトラブルシューティング | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) を参照してください。









