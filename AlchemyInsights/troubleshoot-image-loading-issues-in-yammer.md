---
title: Yammer での画像の読み込みに関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690248"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Yammer での画像の読み込みに関する問題のトラブルシューティング

Yammerの写真とファイルのプレビューで問題が発生した場合は、問題がすべてのユーザーに発生するかどうか、モバイルデバイスで発生するかどうか、および添付ファイルをアップロードする時に再現できるかを確認してトラブルシューティングします。  

**プロフィール写真の問題**  

エンドユーザーが Microsoft 365 経由で Yammer にサインインする場合、プロフィール写真を含むプロファイルを変更する必要があります。 ユーザーがプロファイルの更新を許可していない場合、管理者がユーザーの代わりに更新を行うことができます。 詳細については、「[Office Delve でプロファイルを表示して更新する](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)」を参照してください。

プロファイル写真などのプロファイル編集の詳細については、[ Yammerプロファイルの変更と設定 ](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851) を参照してください。 

更新されたプロファイルの写真は、プロファイルの属性とは違う方法で同期されます。 ユーザーは、自分のプロファイル写真を同期するためにサインインする必要があります。 詳しくは、[ユーザー プロファイルの画像は Office 365 から Yammer に更新されますか ?](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)を参照してください。

Yammer のユーザーライフサイクルの詳細については、[Yammer ユーザーをライフサイクルを通じて Office 365 から管理する](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)を参照してください。  

Microsoft 365 のプロファイル画像同期の詳細については、[「Microsoft 365のプロファイル画像の同期」](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)を参照してください。  

**ドキュメントのプレビューとサムネイル画像の問題**  

ファイルまたは画像が Yammer に投稿されると、プレビューが表示されない理由は次のとおりです: 

- ファイルが破損しているため処理することができません。
- ファイルがまだ SharePoint Online にアップロードされていない、または Yammer がその他の理由で無効なメタデータを持っています。
- プレビューイメージの読み込みに必要な URL はブロックされます。
- ユーザーが投稿前にファイルプレビューを削除しました。
- サービスの問題により、プレビューが生成されませんでした。

**注** プレビューのリンクとファイルのアップロードは異なる動作をする場合があります。 インターネット上のファイルへのリンクまたは追加の認証が必要なリンクは、正しく表示されない場合があります。

詳しくは、[「Yammer メッセージにファイルまたは画像を添付する」](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)をご覧ください。 