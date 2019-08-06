---
title: Teams をスタンドアロンまたは新規または既存の Office インストールとして展開する
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/01/2019
ms.locfileid: "36180402"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Teams をスタンドアロンまたは新規または既存の Office インストールとして展開する

Microsoft Teams は、Office 365 ProPlus、Office 365 Business、および Office for Mac の***新規インストール***の一部として追加されました。 詳細については、「 [Office の新規インストールにいつ Microsoft Teams が組み込まれ始めますか?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus) 」を参照してください。

また、月次チャネルのバージョン1906以降では、既存のインストールを最新バージョンに更新するときに、Windows を実行しているデバイスに Teams が既存の Office 365 ProPlus (および Office 365 Business) に***追加***されます。 詳細については、「 [Office の既存のインストールについて](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)」を参照してください。

> [!NOTE]
> このロールアウトスケジュールを待機する必要がない場合は、次の[手順](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) に従うことによって、またはユーザーが自分のために teams をインストールできる [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)ようにすることで、teams をユーザーに対してスタンドアロンとして展開できます。

組織で Teams を展開する準備ができていない場合は、Office の[新規](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)または[既存](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)のインストールから***teams を除外***するための手順を実行します。 Teams をインストールする必要があるが、インストール後に Teams を自動的に開始したくない場合は、「[インストール後に Microsoft teams が自動的に開始](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)されないようにする」を参照してください。

Windows を実行しているデバイスから***Teams をアンインストール***するには、「 [uninstall Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)」を参照してください。 複数のターゲットコンピューターまたはユーザーから Microsoft Teams をクリーンアップするには、「 [Microsoft teams の展開のクリーンアップ](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)」を参照してください。

共有コンピューター、リモートデスクトップサービス (RDS)、または仮想デスクトップインフラストラクチャ (VDI) を使用している場合は、「 [Microsoft Teams での共有のコンピューターおよび VDI 環境](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)」を参照してください。

Office for Mac を使用している場合は、「 [mac での Microsoft Teams のインストール](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)」を参照してください。

> [!NOTE]
> Teams をインストールすると、新しい機能と品質更新プログラムにより、ほぼ2週間ごと[に自動的に更新さ](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)れます。 