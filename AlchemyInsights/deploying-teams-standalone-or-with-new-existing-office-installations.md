---
title: Teams をスタンドアロンとして、または新規または既存の Offic eインストールで展開する
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806764"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Teams をスタンドアロンとして、または新規または既存の Office インストールで展開する

Microsoft Teams は、Microsoft 365 Apps for enterprise、Microsoft 365 Apps for business、および Office for Mac の***新規インストール***に含まれるようになりました。 詳細については、「[Microsoft Teams は、いつ Office の新規インストールに含まれるようになりますか?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)」を参照してください。

さらに、現在のチャネルのバージョン 1906 以降、Windows を実行しているデバイスで既存のインストールを最新バージョンに更新する際に、Teams が Microsoft 365 Apps for enterprise (および Microsoft 365 Apps for business) の***既存のインストールに追加***されるようになります。 詳細については、「[既存の Office のインストールについて](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)」を参照してください。

> [!NOTE]
> この展開スケジュールを待たない場合は、[次の手順に従って](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) 、ユーザーに Teams をスタンドアロンとして展開することができます。または、ユーザーが  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) から自分で Teams をインストールすることもできます。

組織が Teams を展開する準備ができていない場合、Office の[新規](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps)または[既存](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)のインストールから ***Teams を除外***する手順があります。 Teams をインストールする必要があるが、インストール後、ユーザーに対して Teams が自動的に起動されないようにする場合は、「[インストール後に Microsoft Teams の自動起動を回避する](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)」を参照してください。

Windows を実行しているデバイスから ***Teams をアンインストール***するには、「[Microsoft Teams のアンインストール](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)」を参照してください。 複数のターゲット コンピューターまたはユーザーから Microsoft Teams をクリーンアップするには、「[Microsoft Teams の展開のクリーンアップ](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)」を参照してください。

共有コンピューター、リモート デスクトップ サービス (RDS) または仮想デスクトップ インフラストラクチャ (VDI) を使用している場合は、「[Microsoft Teams での共有コンピューターおよび VDI 環境](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)」を参照してください。

Office for Mac を使用している場合は、「[Microsoft Teams の Mac へのインストール](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)」を参照してください。

> [!NOTE]
> インストール後の Teams は、約 2 週間ごとに新しい機能と品質の更新プログラムによって[自動的に更新](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)されます。 