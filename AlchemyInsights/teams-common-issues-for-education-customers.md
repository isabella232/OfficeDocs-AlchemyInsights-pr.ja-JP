---
title: 教育機関のお客様向け Teams の一般的な問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: d61d4484c720db51e7377201067008192940d1f8
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43739441"
---
# <a name="teams-common-issues-for-education-customers"></a>教育機関のお客様向け Teams の一般的な問題

**教育機関のお客様**:

リモート学習をサポートするための Teams の展開でサポートが必要な場合は、[FastTrack センター](https://www.microsoft.com/fasttrack)にアクセスして、要求を送信してください。 Teams の教育機関のお客様には、次のような一般的な問題があります。

- 「**使い損ねていますよ。**」というメッセージが表示されますか? 「[学校向けに Microsoft Teams を有効にする](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams)」を確認してください。 EDU テナントにおいて、既定では Microsoft Teams は有効になっていません。最初に、Teams を有効にする必要があります。

- **Teams は初めてですか?** 「[Office 365 のリモート教育と学習](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4)」を参照して、学校向けのセットアップに関する最新のガイダンスやトレーニング計画、仮想授業、生徒とのコンテンツの共有について確認してください。

- Teams を有効にすると、ユーザーは Teams を実行できるようになります。[デスクトップ クライアント](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client)または[モバイル クライアント](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients)をインストールする方法と、https://teams.microsoft.com でブラウザーから実行する方法があります。

- **Teams のゲスト アクセスを有効にする**: [Teams のゲスト アクセス チェックリスト](https://docs.microsoft.com/microsoftteams/guest-access-checklist)を確認し、すべての手順が完了していることを確認します。
    - [Microsoft Teams でのゲスト アクセスについて](https://docs.microsoft.com/microsoftteams/guest-access)
    - [セットアップ – Microsoft Teams のゲスト アクセスのチェックリスト](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [ゲストがチームに参加する方法](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams の会議とダイヤルイン**: Microsoft Teams での電話会議の有効化またはセットアップに関してサポートが必要ですか? このユーザーを最近作成しましたか? そうであれば、設定が有効になるまで、2 から 24 時間待つ必要があります。 そのユーザーに電話会議のライセンスが与えられ、既定の有料電話番号があることを確認するには、次のようにします:
    1. アクティブなユーザーに移動し、該当するユーザーを選択します。
    2. 管理センター バージョンに応じて、**[ライセンスとアプリ]** を選択するか、**製品ライセンス**の **[編集]** をクリックします。
    3. ユーザーに、電話会議、Microsoft Teams、および Skype for Business Online (プラン 2) 用に選択したライセンスがあることを確認します。
    4. ユーザー管理センターで、**[すべて表示]**、**[Teams]** の順にクリックします。
    5. Microsoft Teams 管理センターで、**[従来のポータル]** をクリックします。
    6. Skype for Business 管理センターで、**[電話会議]**、**[ユーザー]** の順にクリックします。
    7. 該当するユーザーを選択し、そのユーザーに既定の有料電話番号があることを確認します。

    詳細については、「[通話プラン](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365)」を参照するか、ライセンス関連の質問について Microsoft コマース課金チームにお問い合わせください。

    その他のリソース

    - [Microsoft Teams でのミーティングと会議](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [電話会議](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **会議ポリシー**: 会議ポリシーは、組織内のユーザーによってスケジュールされた会議への参加者が利用できる機能を制御するために使用されます。 ポリシーを作成して変更を行ってから、ユーザーをポリシーに割り当てることができます。

    - **会議の変更または作成**: 会議ポリシーを変更または作成するには、**Microsoft Teams 管理センターにアクセスし、[会議]、[会議ポリシー]** の順に移動します。 一覧からポリシーを選択するか、**[追加]** をクリックします。 新しいポリシーを作成する場合は、名前と説明を追加します。 名前に特殊文字を含めたり、64 文字より長くしたりすることはできません。 設定を選び、**[保存]** をクリックします。 
    
        たとえば、多数のユーザーがいて、会議に必要な帯域幅を制限するとします。 「制限された帯域幅」という名前の新しいカスタム ポリシーを作成し、次の設定を無効にできます。

        **[オーディオとビデオ]** で、
        - **[クラウド記録を許可する]** を無効にします。
        - **[IP のビデオを許可する]** を無効にします。

        **[コンテンツの共有]** で、

        - 画面共有モードを無効にします。
        - **[ホワイトボードを許可]** を無効にします。
        - **[メモの共有を許可する]** を無効にします。

        その後、**ポリシーをユーザーに割り当てます**。

    1. Microsoft Teams 管理センターの左側のナビゲーションで、**[ユーザー]** に移動してユーザーをクリックします。
    2. ユーザー名の左側をクリックしてユーザーを選択し、**[編集を設定する]** をクリックします。
    3. **[会議ポリシー]** で割り当てるポリシーを選択し、**[適用]** をクリックします。

    一度に複数のユーザーにポリシーを割り当てる方法については、「[一括で Teams のユーザー設定を編集する](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk)」を参照してください。

    または、以下の操作を実行できます。
    1. Microsoft Teams 管理センターの左側のナビゲーションで、**[会議] > [会議ポリシー]** の順に移動します。
    2. ポリシー名の左側をクリックしてポリシーを選びます。
    3. **[ユーザーの管理]** をクリックします。
    4. **[ユーザーを管理する]** ウィンドウで、表示名またはユーザー名でユーザーを検索し、名前を選択して **[追加]** をクリックします。 追加するユーザーごとに、この手順を繰り返します。
    5. ユーザーの追加が完了したら、**[保存]** をクリックします。

- **表示されないダイヤル パッドのトラブルシューティング**:
    - ユーザーに [Teams ライセンス](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses)が割り当てられていることを確認します。
    - ユーザーに[通話プラン](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page)が割り当てられていることを確認します。
    - [エンタープライズ VoIP](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail) に対してユーザーを有効にします。

- **Teams サインインのトラブルシューティング:** 最初に、[Microsoft Teams サービスが正常である](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth)ことを確認します。 次に一般的なエラー コードを確認し、「[Microsoft Teams へのサインインで問題が起きるのはなぜですか。](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)」を参照します。 「[Microsoft Teams での ID モデルと認証](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication)」の確認が必要となる場合もあります。
