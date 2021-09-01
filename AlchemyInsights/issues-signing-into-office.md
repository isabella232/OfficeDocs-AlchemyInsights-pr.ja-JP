---
title: Microsoft 365 アプリへのサインインに関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744651"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Microsoft 365 アプリへのサインインに関する問題

注: 以前のバージョンの Windows (Windows 7 SP1、Windows Server 2008 R2 など) を使用している場合は、[簡単な修正プログラム](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi)を使用して TLS 1.2 を既定として有効にします。 詳細については、「[Windows の WinHTTP で TLS 1.1 および TLS 1.2 を既定のセキュリティで保護されたプロトコルとして有効にするための更新プログラム](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)」を参照してください。

Microsoft 365 アプリに関するサインインの問題を修正するには、問題が発生しているコンピューターで次のオプションを試してみてください。  

- Windows の場合は、「[Recommendations on resolving common sign-in issues (サインインに関する一般的な問題の解決についての推奨事項)](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)」を参照してください
- Mac の場合は、「[Office 2016 for Mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください

Windows コンピューターについての **ヒント**、Office の一般的なサインインの問題を診断して、自動的に修正することができます。 **[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA-OfficeSignInScenario)** をダウンロードして実行し、自動化ツールを使用します。

**注:** サインインやアクティベーションの問題を解決するために先進認証 (ADAL) や Web アカウント管理 (WAM) を無効にすることは、**推奨されていません**。 Office 2013 を使用し Microsoft 365 へと接続する際にエラーが発生した場合は、Office クライアントの[先進認証が有効](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)になっていることを確認します。

具体的なトラブルシューティングの手順については、以下をご覧ください。

「[Windows 10 の Office 2016 ビルド16.0.7967 に更新後のサインインにおける接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」  

「[You can't sign in to your organizational account such as Office 365, Azure, or Intune (Office 365、Azure、Intune などの組織アカウントにサインインできない)](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)」

「[How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune (Office 365、Azure、または Intune にサインインできない非ブラウザー アプリのトラブルシューティング)](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)」

「[Repeatedly prompted for credentials in Office (Office で資格情報を繰り返し要求される)](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)」