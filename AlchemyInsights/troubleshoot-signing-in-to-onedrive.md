---
title: OneDrive へのサインインに関するトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8283"
- "9004614"
ms.openlocfilehash: a3ad6d9769dab948cb83c04232bb3d8e937a5dc2
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2021
ms.locfileid: "50257017"
---
# <a name="troubleshoot-signing-in-to-onedrive"></a>OneDrive へのサインインに関するトラブルシューティング

この記事では、以下のシナリオについて説明します。

- OneDrive 同期クライアントへのサインインに関するトラブルシューティング
- OneDrive for Business サイトへのサインインに関するトラブルシューティング

**OneDrive 同期クライアントへのサインインに関するトラブルシューティング**

- サイトにアクセスして OneDrive または SharePoint サイトにサインインし、サイトのメニュー バーの上部にある **[同期]** ボタンをクリックします。
- OneDrive.com ではなく、OneDrive for Business にサインインしていることを確認してください。 アクセスする URL が onedrive.live.com で始まる場合、それは OneDrive for Business の場所ではありません。 確実に OneDrive for Business にサインインする簡単な方法は、このリンク https://portal.office.com/onedrive を使用し、職場または学校のアカウントを使用してログオンすることです。
- 問題が解消されない場合は、[OneDrive のリセット](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c)を検討してください。
- [アカウントを OneDrive からリンク解除](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1)して、OneDrive または SharePoint サイトにサインインし、サイトのメニュー バーの上部にある **[同期]** ボタンをクリックします。

**OneDrive for Business サイトへのサインインに関するトラブルシューティング**

- OneDrive.com ではなく、OneDrive for Business にサインインしていることを確認してください。 アクセスする URL が onedrive.live.com で始まる場合、それは OneDrive for Business の場所ではありません。 確実に OneDrive for Business にサインインする簡単な方法は、このリンク https://portal.office.com/onedrive を使用し、職場または学校のアカウントを使用してログオンすることです。
- Delve プロファイル ページにリダイレクトされた場合、Microsoft 365 管理者は、[OneDrive for Business サイトを作成する権利をユーザーに付与する](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0)必要があります。
- [Microsoft Edge の InPrivate ブラウズ](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc) (または別のブラウザーの同様の機能) を使用して、OneDrive サイトにアクセスできるかどうかをテストします。
    - InPrivate ブラウズが機能する場合は、[Microsoft Edge で閲覧データをクリアする](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4) (または別のブラウザーの同様の操作を行う) 必要がある場合があります。

**OneDrive と同期するための Office へのサインインに関するトラブルシューティング**

**"アップロードはブロックされました"**、**"サインインしてこのファイルを保存"**、または **"コピーを保存"** というエラー メッセージが表示される場合は、[Office 接続済みサービスから OneDrive を削除して再接続する](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8)必要があります。

**その他のトラブルシューティングのヒント**

グローバル管理者、ライセンス管理者、またはユーザー管理者の場合は、[影響を受けるユーザーに正しいライセンスを割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)てください。

