---
title: Intune でメール プロファイルを使用する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919428"
---
# <a name="using-email-profiles-with-intune"></a>Intune でメール プロファイルを使用する

Intune を使用すると、複数のデバイス プラットフォームでネイティブ (組み込み) のメール クライアントのメール プロファイルを作成して展開することができます。

既存のプロファイルの存在の処理方法やメール プロファイルを削除する方法など、メール プロファイルに関するいくつかの制限事項の詳細については、「[Add email settings to devices using Intune (Intune を使用してメール設定をデバイスに追加する)](https://docs.microsoft.com/intune/email-settings-configure)」を参照してください。

各デバイス プラットフォーム用にメール プロファイルを作成する方法の詳細については、次を参照してください。

[Android device settings to configure email, authentication, and synchronization in Intune (Intune でメール、認証、同期を構成するための Android デバイスの設定)](https://docs.microsoft.com/intune/email-settings-android)  
[Add e-mail settings for iOS and iPadOS devices in Microsoft Intune (Microsoft Intune で iOS デバイスおよび iPadOS デバイス用のメール設定を追加する)](https://docs.microsoft.com/intune/email-settings-ios)  
[Email profile settings in Microsoft Intune for devices running Windows Phone 8.1 (Microsoft Intune での、Windows Phone 8.1 を実行するデバイス用のメール プロファイル設定)](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Email profile settings for devices running Windows 10 in Microsoft Intune (Microsoft Intune での、Windows 10 を実行するデバイス用のメール プロファイル設定)](https://docs.microsoft.com/intune/email-settings-windows-10)

**同期に関する一般的な問題**

**Android メール プロファイルの KNOX があるために、ユーザーの連絡先、カレンダー、タスクがユーザーのデバイスに同期されない。**

Android KNOX メール プロファイルの KNOX では、デバイスに同期するコンテンツ タイプを管理者が決定することができ、同期する場合はそれぞれのタイプを有効に設定します。

[**Not configured (未構成)**] (既定) に設定されているコンテンツ タイプは、自動的には同期されません。 ユーザーは、希望するコンテンツ タイプをデバイス上で直接手動で有効にできますが、その構成は Intune ポリシーの設定により上書きされ、そのコンテンツ タイプの同期は停止されます。

